## Favorite books

This request will get your favorite books.
(See add_favorite_request.md on how to add these)

URL: `/api/Favorite/`

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
    "Bibs": [
        {
            "BibId": "347324",
            "StandardNumber": null,
            "Title": "Naruto. 1 /",
            "Author": "Kishimoto, Masashi.",
            "Type": "Teksti",
            "Publisher": "Helsinki Sangatsu manga 2008.",
            "PublishingYear": "2008",
            "Edition": null,
            "ImageUrl": "http://armas.btj.fi/request.php?id=640a18a2c546fb58&pid=9789521610431&qtype=m&ftype=04&error=1",
            "Html": null,
            "Url": "https://kerava.verkkokirjasto.fi/web/arena/results?p_p_id=crDetailWicket_WAR_arenaportlets&p_r_p_687834046_search_item_id=347324"
        }
    ],
    "Status": 1,
    "Message": null,
    "ErrorMessage": null,
    "Copyright": "Copyright (c) 2016-2018 Enisoft Ltd. This interface is for Enisoft's apps' private use only and other use is prohibited."
}`
