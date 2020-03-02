## Loans

To get your active loans, we will need to do a GET request.

URL: `/api/Loan/`

#### Disclaimer
Remember to URL Encode every parameter's value!

#### Parameters

- `apikey` Find it in the `apikey` file
- `deviceid` Parameter `DeviceId` from the login response
- `token` Authorization token from them login response
- `language` Not required as a value, can be `en`, `fi`, `sv`,`ru` or empty. As long the `language` parameter exists, it will work

#### Response
 ###### Statuses:
 	- Available for pickup = 1,
	- Overdue = 2,
	- Charged = 4,
	- Fine = 8,
	- Recall = 10,
	- Unavailable to pickup = 20,
	- Renewed = 40,
	- Not renewed = 80
    - 
`
{
    "Items": [
        {
            "Status": 0,
            "StatusText": null,
            "ImageUrl": "http://armas.btj.fi/request.php?id=640a18a2c546fb58&pid=9781444792492&qtype=m&ftype=04&error=1",
            "StandardNumber": null,
            "RenewStatus": null,
            "RenewStatusText": null,
            "HoldDate": null,
            "ExpirationDate": null,
            "DueDate": "2020-03-10T00:00:00",
            "PickupLocationText": null,
            "ItemId": "4085782",
            "BibId": "432802",
            "Barcode": null,
            "ContextId": "4085782",
            "Title": "Google : how Google works ",
            "Author": "Schmidt, Eric.",
            "MediaTypeText": "Teksti",
            "CirculationStatus": 4,
            "HoldQueueLength": 0,
            "ItemProperties": null
        }
    ],
    "PatronStatus": 0,
    "Currency": null,
    "FeeAmount": null,
    "HoldItemsCount": 0,
    "OverdueItemsCount": 0,
    "ChargedItemsCount": 0,
    "FineItemsCount": 0,
    "RecallItemsCount": 0,
    "UnavailableHoldsCount": 0,
    "Status": 1,
    "Message": "",
    "ErrorMessage": "",
    "Copyright": "Copyright (c) 2016-2018 Enisoft Ltd. This interface is for Enisoft's apps' private use only and other use is prohibited."
}`
