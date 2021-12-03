---
title: inputGroupCallStream
description: inputGroupCallStream attributes, type and example
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: inputGroupCallStream  
[Back to constructors index](index.md)



### Attributes:

| Name     |    Type       | Required |
|----------|---------------|----------|
|call|[InputGroupCall](../types/InputGroupCall.md) | Yes|
|time\_ms|[long](../types/long.md) | Yes|
|scale|[int](../types/int.md) | Yes|
|video\_channel|[int](../types/int.md) | Optional|
|video\_quality|[int](../types/int.md) | Optional|



### Type: [InputFileLocation](../types/InputFileLocation.md)


### Example:

```php
$inputGroupCallStream = ['_' => 'inputGroupCallStream', 'call' => InputGroupCall, 'time_ms' => long, 'scale' => int, 'video_channel' => int, 'video_quality' => int];
```  


Or, if you're into Lua:

```lua
inputGroupCallStream={_='inputGroupCallStream', call=InputGroupCall, time_ms=long, scale=int, video_channel=int, video_quality=int}

```

