---
title: updateChannelAvailableMessages
description: The history of a [channel/supergroup](https://core.telegram.org/api/channel) was hidden.
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: updateChannelAvailableMessages  
[Back to constructors index](index.md)



The history of a [channel/supergroup](https://core.telegram.org/api/channel) was hidden.

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|channel\_id|[long](../types/long.md) | Yes|
|available\_min\_id|[int](../types/int.md) | Yes|Identifier of a maximum unavailable message in a channel due to hidden history.|



### Type: [Update](../types/Update.md)


### Example:

```php
$updateChannelAvailableMessages = ['_' => 'updateChannelAvailableMessages', 'channel_id' => long, 'available_min_id' => int];
```  


Or, if you're into Lua:

```lua
updateChannelAvailableMessages={_='updateChannelAvailableMessages', channel_id=long, available_min_id=int}

```

