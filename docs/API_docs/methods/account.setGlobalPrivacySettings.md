---
title: "account.setGlobalPrivacySettings"
description: "Set global privacy settings"
grand_parent: "Telegram RPC API"
parent: "Methods"
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/account_setGlobalPrivacySettings.html
---
# Method: account.setGlobalPrivacySettings
[Back to methods index](index.html)



Set global privacy settings

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|settings|[GlobalPrivacySettings](/API_docs/types/GlobalPrivacySettings.html) | Global privacy settings | Yes|


### Return type: [GlobalPrivacySettings](/API_docs/types/GlobalPrivacySettings.html)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$GlobalPrivacySettings = $MadelineProto->account->setGlobalPrivacySettings(['settings' => GlobalPrivacySettings, ]);
```

### Errors

| Code | Type     | Description   |
|------|----------|---------------|
|400|AUTOARCHIVE_NOT_AVAILABLE|The autoarchive setting is not available at this time: please check the value of the [autoarchive_setting_available field in client config &raquo;](https://core.telegram.org/api/config#client-configuration) before calling this method.|

