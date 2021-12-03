---
title: phone.getGroupCall
description: phone.getGroupCall parameters, return type and example
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/phone_getGroupCall.html
---
# Method: phone.getGroupCall
[Back to methods index](index.md)



### Parameters:

| Name     |    Type       | Required |
|----------|---------------|----------|
|call|[InputGroupCall](../types/InputGroupCall.md) | Yes|
|limit|[int](../types/int.md) | Yes|


### Return type: [phone.GroupCall](../types/phone.GroupCall.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$phone_GroupCall = $MadelineProto->phone->getGroupCall(['call' => InputGroupCall, 'limit' => int, ]);
```

Or, if you're into Lua:

```lua
phone_GroupCall = phone.getGroupCall({call=InputGroupCall, limit=int, })
```
