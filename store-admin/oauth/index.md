# Connect OAuth

- [Introduction](#introduction)
- [Authorization](#authorization)
- [Access Token](#access-token)
- [Refresh Token](#refresh-token)

<a name="introduction"></a>
## introduction

To connect to YouCan API, you can use the standard [OAuth 2](https://oauth.net/2/) to get an access token.

<a name="authorization"></a>
## Authorization

The first step is to redirect to YouCan for getting an authorization code.

```
https://seller-area.youcan.shop/admin/oauth/authorize?client_id=1&redirect_uri=https://myapp.com/callback&response_type=code&scope=*
```
<a name="access-token"></a>
## Access Token

After the seller answer the authorization popup, he will be redirected to the specified redirect uri (`https://myapp.com/callback`) where you can exchange the authorization code for an access token. Here's an example using Laravel:

```php
Route::get(
    '/callback',
    function (Request $request) {
        // If an error occurred or seller rejected authorization
        if ($request->has('error')) {
            if ($request->get('error') === 'access_denied') {
                return 'You canceled the request';
            }

            return "an error occurred";
        }

        $http = new GuzzleHttp\Client;

        $response = $http->post(
            'https://seller-area.youcan.shop/admin/oauth/token',
            [
                'form_params' => [
                    'grant_type'    => 'authorization_code',
                    'client_id'     => 1,
                    'client_secret' => '<CLIENT SECRET>',
                    'redirect_uri'  => 'https://myapp.com/callback',
                    'code'          => $request->get('code'),
                ],
                'http_errors' => false,
            ]
        );

        return json_decode((string)$response->getBody(), true);
    }
);
```

Response:

```json
{
    "token_type": "Bearer",
    "expires_in": 1295999,
    "access_token": "<ACCESS TOKEN>",
    "refresh_token": "<REFRESH TOKEN>"
}
```

As an alternative, you can request, regenerate and revoke an access token from your seller-area in [Settings > Developer Settings](https://seller-area.youcan.shop/admin/settings/developer)

<a name="refresh-token"></a>
## Refresh Token 

Ideally the access token has a lifetime of one year, unless it's revoked. You can refresh it using the `refresh_token` attribute you got from the response. Here's an example of how to refresh it:

```php
$http = new GuzzleHttp\Client;

$response = $http->post(
    'http://seller-area.youcan.shop/admin/oauth/token',
    [
        'form_params' => [
            'grant_type'    => 'refresh_token',
            'client_id'     => 1,
            'client_secret' => '<CLIENT SECRET>',
            'refresh_token'  => '<REFRESH TOKEN>',
        ],
        'http_errors' => false,
    ]
);
```
