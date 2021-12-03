---
title: phone.inviteToGroupCall
description: phone.inviteToGroupCall parameters, return type and example
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/phone_inviteToGroupCall.html
---
# Method: phone.inviteToGroupCall
[Back to methods index](index.md)



### Parameters:

| Name     |    Type       | Required |
|----------|---------------|----------|
|call|[InputGroupCall](../types/InputGroupCall.md) | Yes|
|users|Array of [Username, chat ID, Update, Message or InputUser](../types/InputUser.md) | Yes|


### Return type: [Updates](../types/Updates.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Updates = $MadelineProto->phone->inviteToGroupCall(['call' => InputGroupCall, 'users' => [InputUser, InputUser], ]);
```

Or, if you're into Lua:

```lua
Updates = phone.inviteToGroupCall({call=InputGroupCall, users={InputUser}, })
```

### Errors

| Code | Type     | Description   |
|------|----------|---------------|
|403|GROUPCALL_FORBIDDEN|The group call has already ended|

