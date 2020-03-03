## Search

To search books and other items to loan, we will need to do a GET request.

URL: `/api/Search/`

#### Disclaimer
Remember to URL Encode every parameter's value!

#### Parameters

- `apikey` Find it in the `apikey` file
- `deviceid` Parameter `DeviceId` from the login response
- `token` Authorization token from them login response
- `language` Required, should be `en`, `fi`, `sv` or `ru`.
- `terms` Your search query, i.e "how google works"

#### Response
`
{
    "Bibs": [
        {
            "BibId": "432802",
            "StandardNumber": "9781444792492",
            "Title": "Google : how Google works ",
            "Author": "Schmidt, Eric.",
            "Type": "Teksti",
            "Publisher": "",
            "PublishingYear": "2015",
            "Edition": "",
            "ImageUrl": "http://armas.btj.fi/request.php?id=640a18a2c546fb58&pid=9781444792492&qtype=m&ftype=04&error=1",
            "Html": "",
            "Url": "https://kerava.verkkokirjasto.fi/web/arena/results?p_p_id=crDetailWicket_WAR_arenaportlets&p_r_p_687834046_search_item_id=432802"
        }
    ],
    "Hits": null,
    "Status": 1,
    "Message": "",
    "ErrorMessage": "",
    "Copyright": "Copyright (c) 2016-2018 Enisoft Ltd. This interface is for Enisoft's apps' private use only and other use is prohibited."
}`
