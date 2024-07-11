```/rest/api/v1/WebService/CheckSmsStatus``` :
```
curl -X 'GET' \
  'https://gw.ghasedak.me/rest/api/v1/WebService/CheckSmsStatus?Ids=2366799&Type=1' \
  -H 'accept: text/plain' \
  -H 'ApiKey: b7ee4eace78744868fc38b1b7fa90caed21717d4d7bf2c9f483d8abce6c018e1'
```

```/rest/api/v1/WebService/GetAccountInformation``` :
```
curl -X 'GET' \
  'https://gw.ghasedak.me/rest/api/v1/WebService/GetAccountInformation' \
  -H 'accept: text/plain' \
  -H 'ApiKey: b7ee4eace78744868fc38b1b7fa90caed21717d4d7bf2c9f483d8abce6c018e1'
```

```/rest/api/v1/WebService/GetReceivedSmses``` :
```
curl -X 'GET' \
  'https://gw.ghasedak.me/rest/api/v1/WebService/GetReceivedSmses?LineNumber=210002100&IsRead=true' \
  -H 'accept: text/plain' \
  -H 'ApiKey: b7ee4eace78744868fc38b1b7fa90caed21717d4d7bf2c9f483d8abce6c018e1'
```

```/rest/api/v1/WebService/GetReceivedSmsesPaging``` :
```
curl -X 'GET' \
  'https://gw.ghasedak.me/rest/api/v1/WebService/GetReceivedSmsesPaging?LineNumber=210002100&IsRead=true' \
  -H 'accept: text/plain' \
  -H 'ApiKey: b7ee4eace78744868fc38b1b7fa90caed21717d4d7bf2c9f483d8abce6c018e1'
```

```/rest/api/v1/WebService/GetOtpTemplateParameters``` :
```
curl -X 'GET' \
  'https://gw.ghasedak.me/rest/api/v1/WebService/GetOtpTemplateParameters?TemplateName=oldOTP' \
  -H 'accept: text/plain' \
  -H 'ApiKey: b7ee4eace78744868fc38b1b7fa90caed21717d4d7bf2c9f483d8abce6c018e1'
```

```/rest/api/v1/WebService/SendSingleSMS```
```
curl -X 'POST' \
  'https://gw.ghasedak.me/rest/api/v1/WebService/SendSingleSMS' \
  -H 'accept: text/plain' \
  -H 'ApiKey: b7ee4eace78744868fc38b1b7fa90caed21717d4d7bf2c9f483d8abce6c018e1' \
  -H 'Content-Type: application/json' \
  -d '{
  "sendDate": "2024-07-11T17:36:09.500Z",
  "lineNumber": "210002100",
  "receptor": "09120581875",
  "message": "strin2g",
  "clientReferenceId": "stringfsdfsdf",
  "udh": false
}'
```

```/rest/api/v1/WebService/SendBulkSMS```
```
curl -X 'POST' \
  'https://gw.ghasedak.me/rest/api/v1/WebService/SendBulkSMS' \
  -H 'accept: text/plain' \
  -H 'ApiKey: b7ee4eace78744868fc38b1b7fa90caed21717d4d7bf2c9f483d8abce6c018e1' \
  -H 'Content-Type: application/json' \
  -d '{
  "sendDate": "2024-07-11T18:17:44.980Z",
  "lineNumber": "210002100",
  "receptors": [
    "09120581875"
  ],
  "message": "string",
  "clientReferenceId": "string",
  "isVoice": false,
  "udh": false
}'
```

```/rest/api/v1/WebService/SendPairToPairSMS```
```
curl -X 'POST' \
  'https://gw.ghasedak.me/rest/api/v1/WebService/SendPairToPairSMS' \
  -H 'accept: text/plain' \
  -H 'ApiKey: b7ee4eace78744868fc38b1b7fa90caed21717d4d7bf2c9f483d8abce6c018e1' \
  -H 'Content-Type: application/json' \
  -d '{
  "items": [
    {
      "lineNumber": "210002100",
      "receptor": "09120581875",
      "message": "string",
      "clientReferenceId": "sdsdfdsftring",
      "sendDate": "2024-07-11T17:54:32.973Z"
    },
    {
      "lineNumber": "210002100",
      "receptor": "09120581875",
      "message": "string3",
      "clientReferenceId": "sdsfdsfsddfdsftring",
      "sendDate": "2024-07-11T17:54:32.973Z"
    }
  ],
  "udh": true
}'
```

```/rest/api/v1/WebService/SendOtpWithParams```
```
curl -X 'POST' \
  'https://gw.ghasedak.me/rest/api/v1/WebService/SendOtpWithParams' \
  -H 'accept: text/plain' \
  -H 'ApiKey: b7ee4eace78744868fc38b1b7fa90caed21717d4d7bf2c9f483d8abce6c018e1' \
  -H 'Content-Type: application/json' \
  -d '{

  "receptors": [
    {
      "mobile": "09120581875",
      "clientReferenceId": "stghfghgfrxsding"
    }
  ],
  "templateName": "oldOTP",
  "param1": "fgfhfg",
  "param2": "hfghgf",
  "param3": "string",
  "param4": "string",
  "param5": "string",
  "param6": "string",
  "param7": "string",
  "param8": "string",
  "param9": "string",
  "param10": "string",
  "isVoice": false,
  "udh": false
}'
```

```/rest/api/v1/WebService/SendOtpSMS```
```
curl -X 'POST' \
  'https://gw.ghasedak.me/rest/api/v1/WebService/SendOtpSMS' \
  -H 'accept: text/plain' \
  -H 'ApiKey: b7ee4eace78744868fc38b1b7fa90caed21717d4d7bf2c9f483d8abce6c018e1' \
  -H 'Content-Type: application/json' \
  -d '{
  "sendDate": "2024-07-11T18:16:05.952Z",
  "receptors": [
    {
      "mobile": "09120581875",
      "clientReferenceId": "string"
    }
  ],
  "templateName": "newOTP",
  "inputs": [
    {
      "param": "Name",
      "value": "string"
    },
   {
      "param": "Code",
      "value": "string"
    }
  ],
  "udh": false
}'
```

