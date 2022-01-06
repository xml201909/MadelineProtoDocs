---
title: "channelAdminLogEventActionChangeAvailableReactions"
description: "channelAdminLogEventActionChangeAvailableReactions attributes, type and example"
nav_exclude: true
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: channelAdminLogEventActionChangeAvailableReactions  
[Back to constructors index](index.md)



### Attributes:

| Name     |    Type       | Required |
|----------|---------------|----------|
|prev\_value|Array of [string](../types/string.md) | Yes|
|new\_value|Array of [string](../types/string.md) | Yes|



### Type: [ChannelAdminLogEventAction](../types/ChannelAdminLogEventAction.md)


### Example:

```php
$channelAdminLogEventActionChangeAvailableReactions = ['_' => 'channelAdminLogEventActionChangeAvailableReactions', 'prev_value' => ['string', 'string'], 'new_value' => ['string', 'string']];
```  


Or, if you're into Lua:

```lua
channelAdminLogEventActionChangeAvailableReactions={_='channelAdminLogEventActionChangeAvailableReactions', prev_value={'string'}, new_value={'string'}}

```

