---
title: "phone.joinGroupCallPresentation"
description: "phone.joinGroupCallPresentation parameters, return type and example"
grand_parent: "Telegram RPC API"
parent: "Methods"
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/phone_joinGroupCallPresentation.html
---
# Method: phone.joinGroupCallPresentation
[Back to methods index](index.html)



### Parameters:

| Name     |    Type       | Required |
|----------|---------------|----------|
|call|[InputGroupCall](/API_docs/types/InputGroupCall.html) | Yes|
|params|[DataJSON](/API_docs/types/DataJSON.html) | Yes|


### Return type: [Updates](/API_docs/types/Updates.html)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Updates = $MadelineProto->phone->joinGroupCallPresentation(['call' => InputGroupCall, 'params' => DataJSON, ]);
```

### Errors

| Code | Type     | Description   |
|------|----------|---------------|
|403|PARTICIPANT_JOIN_MISSING|Trying to enable a presentation, when the user hasn't joined the Video Chat with [phone.joinGroupCall](/method/phone.joinGroupCall)|

