## Books waiting for pickup

This request will get your pending books, which should be picked up.

URL: `/api/Hold/`
#### Parameters


- `apikey` Find it in the `apikey` file
- `deviceid` Parameter `DeviceId` from the login response
- `token` Authorization token from them login response
- `language` Required in this request, should be be `en`, `fi`, `sv` or `ru` 

#### Response

`
{
    "Items": [
        {
            "Status": 32,
            "StatusText": "Voimassa",
            "ImageUrl": "http://armas.btj.fi/request.php?id=640a18a2c546fb58&pid=9789511256458&qtype=m&ftype=04&error=1",
            "StandardNumber": null,
            "RenewStatus": null,
            "RenewStatusText": null,
            "HoldDate": "2020-01-29T00:00:00",
            "ExpirationDate": null,
            "DueDate": null,
            "PickupLocationText": null,
            "ItemId": "405180",
            "BibId": "392532",
            "Barcode": null,
            "ContextId": "405180",
            "Title": "Steve Jobs ",
            "Author": "Isaacson, Walter.",
            "MediaTypeText": "Teksti",
            "CirculationStatus": 0,
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
