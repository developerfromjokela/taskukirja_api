## Add a book to the favorites list

This request will add a book to the favorites list. Use *PUT* as a request type.
(See favorite_books_request.md on how to get the list)

URL: `/api/Favorite/`

#### Disclaimer
Remember to URL Encode every parameter's value!

#### Parameters


- `apikey` Find it in the `apikey` file
- `deviceid` Parameter `DeviceId` from the login response
- `token` Authorization token from them login response
- `language` Required in this request, should be be `en`, `fi`, `sv` or `ru` 
- `bibid` Required in this request, value can be originated from: search request, reservations, waiting for pickup, or if there's an string called `BibId`

#### Response

`
{
    "Status": 1,
    "Message": "Suosikki lisätty.",
    "ErrorMessage": "Suosikki lisätty.",
    "Copyright": "Copyright (c) 2016-2018 Enisoft Ltd. This interface is for Enisoft's apps' private use only and other use is prohibited."
}
`
