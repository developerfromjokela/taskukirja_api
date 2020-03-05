## Pickup locations

This request will get the Kerava Library's information and contact information

URL: `/api/Contact/`

#### Disclaimer
Remember to URL Encode every parameter's value!

#### Parameters


- `apikey` Find it in the `apikey` file
- `deviceid` Parameter `DeviceId` from the login response
- `token` Authorization token from them login response
- `language` Required in this request, should be be `en`, `fi`, `sv` or `ru` 
#### Response

`
{
    "Language": "fi",
    "Libraries": [
        {
            "Id": 86078,
            "Name": "Keravan kaupunginkirjasto",
            "Street": "Paasikivenkatu 12",
            "Zip": "04200",
            "City": "Kerava",
            "Lat": "60.40550000",
            "Lon": "25.10306000",
            "Homepage": "https://kerava.verkkokirjasto.fi/web/arena",
            "Email": "kirjasto@kerava.fi",
            "Open": [
                {
                    "Opens": "2020-03-05T08:00:00+02:00",
                    "Closes": "2020-03-05T20:00:00+02:00",
                    "Closed": false
                },
                {
                    "Opens": "2020-03-06T08:00:00+02:00",
                    "Closes": "2020-03-06T18:00:00+02:00",
                    "Closed": false
                },
                {
                    "Opens": "2020-03-07T09:00:00+02:00",
                    "Closes": "2020-03-07T17:00:00+02:00",
                    "Closed": false
                },
                {
                    "Opens": "2020-03-08T00:00:00+02:00",
                    "Closes": null,
                    "Closed": true
                },
                {
                    "Opens": "2020-03-09T08:00:00+02:00",
                    "Closes": "2020-03-09T20:00:00+02:00",
                    "Closed": false
                },
                {
                    "Opens": "2020-03-10T08:00:00+02:00",
                    "Closes": "2020-03-10T20:00:00+02:00",
                    "Closed": false
                },
                {
                    "Opens": "2020-03-11T08:00:00+02:00",
                    "Closes": "2020-03-11T20:00:00+02:00",
                    "Closed": false
                }
            ],
            "PhoneNumbers": [
                {
                    "Name": "Palvelukeskus",
                    "Number": "040 318 2157"
                }
            ],
            "HasPhone": true
        }
    ],
    "Updated": "2020-03-05T12:30:11.135Z",
    "Now": "2020-03-05T14:49:38.6380046+02:00",
    "Status": 1,
    "Message": null,
    "ErrorMessage": null,
    "Copyright": "Copyright (c) 2016-2018 Enisoft Ltd. This interface is for Enisoft's apps' private use only and other use is prohibited."
}`
