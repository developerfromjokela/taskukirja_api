## Pickup locations

This request will get your available pickup locations, when reserving books.

URL: `/api/Hold/PickupLocations`

#### Disclaimer
Remember to URL Encode every parameter's value!

#### Parameters


- `apikey` Find it in the `apikey` file
- `deviceid` Parameter `DeviceId` from the login response
- `token` Authorization token from them login response
- `language` Required in this request, should be be `en`, `fi`, `sv` or `ru` 
- (optional) `bibid` This parameter specifies the book you want to loan.
#### Response

`
{
    "Updated": null,
    "PickupLocations": [
        {
            "Code": "2.101",
            "Name": "Järvenpään kirjasto"
        },
        {
            "Code": "1.002",
            "Name": "Jokelan kirjasto"
        },
        {
            "Code": "1.003",
            "Name": "Kellokosken kirjasto"
        },
        {
            "Code": "3.201",
            "Name": "Keravan kirjasto"
        },
        {
            "Code": "4.302",
            "Name": "Mäntsälän kirjastoauto"
        },
        {
            "Code": "4.301",
            "Name": "Mäntsälän pääkirjasto"
        },
        {
            "Code": "1.005",
            "Name": "Tuusulan Kirjastoauto"
        },
        {
            "Code": "1.001",
            "Name": "Tuusulan pääkirjasto"
        }
    ],
    "Status": 1,
    "Message": null,
    "ErrorMessage": null,
    "Copyright": "Copyright (c) 2016-2018 Enisoft Ltd. This interface is for Enisoft's apps' private use only and other use is prohibited."
}`
