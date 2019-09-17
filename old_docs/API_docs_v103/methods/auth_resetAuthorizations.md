---
title: auth.resetAuthorizations
description: Delete all logged-in sessions.
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: auth.resetAuthorizations  
[Back to methods index](index.md)


Delete all logged-in sessions.



### Return type: [Bool](../types/Bool.md)

### Can bots use this method: **YES**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Bool = $MadelineProto->auth->resetAuthorizations();
```

Or, if you're into Lua:

```lua
Bool = auth.resetAuthorizations({})
```

### Errors

| Code | Type     | Description   |
|------|----------|---------------|
|406|FRESH_RESET_AUTHORISATION_FORBIDDEN|You can't logout other sessions if less than 24 hours have passed since you logged on the current session|
|-503|Timeout|Timeout while fetching data|

