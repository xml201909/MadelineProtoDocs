---
title: account.reportProfilePhoto
description: account.reportProfilePhoto parameters, return type and example
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/account_reportProfilePhoto.html
---
# Method: account.reportProfilePhoto
[Back to methods index](index.md)



### Parameters:

| Name     |    Type       | Required |
|----------|---------------|----------|
|peer|[Username, chat ID, Update, Message or InputPeer](../types/InputPeer.md) | Optional|
|photo\_id|[MessageMedia, Update, Message or InputPhoto](../types/InputPhoto.md) | Optional|
|reason|[ReportReason](../types/ReportReason.md) | Yes|
|message|[string](../types/string.md) | Yes|


### Return type: [Bool](../types/Bool.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Bool = $MadelineProto->account->reportProfilePhoto(['peer' => InputPeer, 'photo_id' => InputPhoto, 'reason' => ReportReason, 'message' => 'string', ]);
```

Or, if you're into Lua:

```lua
Bool = account.reportProfilePhoto({peer=InputPeer, photo_id=InputPhoto, reason=ReportReason, message='string', })
```


## Return value 

If the length of the provided message is bigger than 4096, the message will be split in chunks and the method will be called multiple times, with the same parameters (except for the message), and an array of [Bool](../types/Bool.md) will be returned instead.

