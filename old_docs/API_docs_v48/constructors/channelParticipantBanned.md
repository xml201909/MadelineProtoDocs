---
title: channelParticipantBanned
description: Banned/kicked user
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: channelParticipantBanned  
[Back to constructors index](index.md)



Banned/kicked user

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|left|[Bool](../types/Bool.md) | Optional|Whether the user has left the group|
|peer|[Peer](../types/Peer.md) | Yes|
|kicked\_by|[int](../types/int.md) | Yes|User was kicked by the specified admin|
|date|[int](../types/int.md) | Yes|When did the user join the group|
|banned\_rights|[ChatBannedRights](../types/ChatBannedRights.md) | Yes|Banned [rights](https://core.telegram.org/api/rights)|



### Type: [ChannelParticipant](../types/ChannelParticipant.md)


### Example:

```php
$channelParticipantBanned = ['_' => 'channelParticipantBanned', 'left' => Bool, 'peer' => Peer, 'kicked_by' => int, 'date' => int, 'banned_rights' => ChatBannedRights];
```  


Or, if you're into Lua:

```lua
channelParticipantBanned={_='channelParticipantBanned', left=Bool, peer=Peer, kicked_by=int, date=int, banned_rights=ChatBannedRights}

```

