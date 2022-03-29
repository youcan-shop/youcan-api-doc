# Get Seller Profits

Endpoint: `https://api.youcan.shop/packs`

Method :  `GET`

## Response

[200]

```json
{
    "packs": [
        {
            "id": "04dc5a4d-605b-4984-bf1f-f0f7d31a3b24",
            "name": "Solopreneur",
            "debit_day": 1,
            "is_default": 0,
            "created_at": "2022-03-07 11:35:18",
            "updated_at": "2022-03-07 11:35:18",
            "deleted_at": null,
            "max_users": 1,
            "max_ca": 50000,
            "price": 27,
            "is_selected": false,
            "rates": []
        },
        {
            "id": "0f75a6d8-2f97-4ff5-92d7-f9dd113fc1b4",
            "name": "Starter",
            "debit_day": 1,
            "is_default": 0,
            "created_at": "2022-03-07 11:35:18",
            "updated_at": "2022-03-07 11:35:18",
            "deleted_at": null,
            "max_users": 3,
            "max_ca": 100000,
            "price": 47,
            "is_selected": false,
            "rates": []
        },
        {
            "id": "692254e2-c857-4a39-b707-04fb02e40325",
            "name": "Default",
            "debit_day": 1,
            "is_default": 1,
            "created_at": "2022-03-07 11:35:06",
            "updated_at": "2022-03-07 11:35:06",
            "deleted_at": null,
            "max_users": null,
            "max_ca": null,
            "price": null,
            "is_selected": true,
            "rates": {
                "2": {
                    "id": "3887a2e6-e24d-40bf-b3c0-6016678fd1c8",
                    "min": 0,
                    "max": 39999.99,
                    "type": 2,
                    "value": 0.5,
                    "pack_id": "692254e2-c857-4a39-b707-04fb02e40325",
                    "created_at": "2022-03-07 11:35:06",
                    "updated_at": "2022-03-07 11:35:06",
                    "deleted_at": null
                },
                "0": {
                    "id": "215d5bb2-a813-45ee-b636-2b7fb68a80e7",
                    "min": 40000,
                    "max": 99999.99,
                    "type": 2,
                    "value": 0.3,
                    "pack_id": "692254e2-c857-4a39-b707-04fb02e40325",
                    "created_at": "2022-03-07 11:35:06",
                    "updated_at": "2022-03-07 11:35:06",
                    "deleted_at": null
                },
                "3": {
                    "id": "925b5b51-3d81-4848-aab4-3b5712430803",
                    "min": 100000,
                    "max": 249999.99,
                    "type": 2,
                    "value": 0.24,
                    "pack_id": "692254e2-c857-4a39-b707-04fb02e40325",
                    "created_at": "2022-03-07 11:35:06",
                    "updated_at": "2022-03-07 11:35:06",
                    "deleted_at": null
                },
                "1": {
                    "id": "27db9bf7-06ab-43f0-8e27-6803540812a2",
                    "min": 250000,
                    "max": null,
                    "type": 2,
                    "value": 0.2,
                    "pack_id": "692254e2-c857-4a39-b707-04fb02e40325",
                    "created_at": "2022-03-07 11:35:06",
                    "updated_at": "2022-03-07 11:35:06",
                    "deleted_at": null
                }
            }
        },
        {
            "id": "7f1e1ca0-533e-44fc-bbcf-f3ef43a03feb",
            "name": "Yearly Plan",
            "debit_day": 1,
            "is_default": 0,
            "created_at": "2022-03-07 11:35:24",
            "updated_at": "2022-03-07 11:35:24",
            "deleted_at": null,
            "max_users": null,
            "max_ca": null,
            "price": 970,
            "is_selected": false,
            "rates": []
        },
        {
            "id": "a4bed7a0-34ce-4a93-b934-b4f851454d7d",
            "name": "Entrepreneur",
            "debit_day": 1,
            "is_default": 0,
            "created_at": "2022-03-07 11:35:18",
            "updated_at": "2022-03-07 11:35:18",
            "deleted_at": null,
            "max_users": 6,
            "max_ca": 300000,
            "price": 87,
            "is_selected": false,
            "rates": []
        },
        {
            "id": "a5a1dc40-44c3-4d84-956f-42d4045a6cbe",
            "name": "Unlimited",
            "debit_day": 1,
            "is_default": 0,
            "created_at": "2022-03-07 11:35:24",
            "updated_at": "2022-03-07 11:35:24",
            "deleted_at": null,
            "max_users": null,
            "max_ca": null,
            "price": 300,
            "is_selected": false,
            "rates": []
        },
        {
            "id": "c4fe9487-bea8-443e-bc44-10635f7577a5",
            "name": "Small Medium Enterprise",
            "debit_day": 1,
            "is_default": 0,
            "created_at": "2022-03-07 11:35:18",
            "updated_at": "2022-03-07 11:35:18",
            "deleted_at": null,
            "max_users": 19,
            "max_ca": 1000000,
            "price": 187,
            "is_selected": false,
            "rates": []
        },
        {
            "id": "cc3e4f31-566a-4c0c-9655-a615de83bb3b",
            "name": "WeCan",
            "debit_day": 1,
            "is_default": 0,
            "created_at": "2022-03-07 11:35:18",
            "updated_at": "2022-03-07 11:35:18",
            "deleted_at": null,
            "max_users": null,
            "max_ca": null,
            "price": 570,
            "is_selected": false,
            "rates": []
        }
    ]
}
```