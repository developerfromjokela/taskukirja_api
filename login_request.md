## Login Request

Login request is made using GET request (really? who made this??).
And all parameters are sent as GET parameters:

- `deviceid`: This parameter doesn't matter, as long it exists, it's gonna work
- `userid`: Library card number or username
- `password`: Library card Pin-Code or password
- `language`: This parameter doesn't matter, as long it exists, it's gonna work
- `uri`: This parameter doesn't matter, as long it exists, it's gonna work
- `devicetype`: This is used for the Push notifications, value `4` means Android device
- `apikey`: Find this value in `api_key` file

Example response:
`{
    "Name": "Example user",
    "Token": "{{your_token}}",
    "DeviceId": "{{device_token}}",
    "TokenExpiration": "2020-03-02T01:20:58+02:00",
    "Status": 1,
    "Message": "",
    "ErrorMessage": "",
    "Copyright": "Copyright (c) 2016-2018 Enisoft Ltd. This interface is for Enisoft's apps' private use only and other use is prohibited."
}`

Error response:
`{
    "Message": "Random error message ;-)"
}`

There is some possibility, that the ErrorMessage will be the Error text, so be prepared for this error response:
`{
    "ErrorMessage": "Random error message ;-)"
}`
