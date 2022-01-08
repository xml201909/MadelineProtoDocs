---
title: "messages.deleteChat"
description: "messages.deleteChat parameters, return type and example"
grand_parent: "Telegram RPC API"
parent: "Methods"
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/messages_deleteChat.html
---
# Method: messages.deleteChat
[Back to methods index](index.html)



### Parameters:

| Name     |    Type       | Required |
|----------|---------------|----------|
|chat\_id|[Username, chat ID, Update, Message or InputPeer](/API_docs/types/InputPeer.html) | Optional|


### Return type: [Bool](/API_docs/types/Bool.html)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Bool = $MadelineProto->messages->deleteChat(['chat_id' => InputPeer, ]);
```

### Errors

| Code | Type     | Description   |
|------|----------|---------------|
|400|CHAT_ID_INVALID|The provided chat id is invalid|
|400|PEER_ID_INVALID|The provided peer id is invalid|

