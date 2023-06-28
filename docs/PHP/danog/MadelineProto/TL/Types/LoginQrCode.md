---
title: "danog\\MadelineProto\\TL\\Types\\LoginQrCode: Represents a login QR code."
description: "The `link` public readonly property contains the [QR code login link](https://core.telegram.org/api/links#qr-code-login-links).\nThe `expiry` public readonly property contains the expiry date of the link."
image: "https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png"
parent: "MadelineProto API"

---
# `danog\MadelineProto\TL\Types\LoginQrCode`
[Back to index](../../../../index.html)

> Author: Daniil Gentili <daniil@daniil.it>  
  

Represents a login QR code.  

The `link` public readonly property contains the [QR code login link](https://core.telegram.org/api/links#qr-code-login-links).
The `expiry` public readonly property contains the expiry date of the link.


## Method list:
* [`isExpired(): bool`](#isexpired-bool)
* [`expiresIn(): int`](#expiresin-int)
* [`waitForLoginOrQrCodeExpiration(\Amp\Cancellation|null $customCancellation): ?self`](#waitforloginorqrcodeexpiration-amp-cancellation-null-customcancellation-self)
* [`getQRSvg(int $size, int $margin): string`](#getqrsvg-int-size-int-margin-string)
* [`getQRText(int $margin): string`](#getqrtext-int-margin-string)

## Methods:
### `isExpired(): bool`

Returns true if the QR code has expired and a new one should be fetched.



### `expiresIn(): int`

Returns the number of seconds until the QR code expires.



### `waitForLoginOrQrCodeExpiration(\Amp\Cancellation|null $customCancellation): ?self`

Waits for the user to login or for the QR code to expire.
If the user logins, null is returned.  
  
If the QR code expires, the new QR code is returned.  
  
If cancellation is requested externally through $cancellation, a CancelledException is thrown.

Parameters:

* `$customCancellation`: `\Amp\Cancellation|null` Optional additional cancellation  


#### See also: 
* `\Amp\Cancellation`




### `getQRSvg(int $size, int $margin): string`

Render and return SVG version of QR code.


Parameters:

* `$size`: `int`   
* `$margin`: `int`   



### `getQRText(int $margin): string`

Render and return plain text version of QR code.


Parameters:

* `$margin`: `int`   



---
Generated by [danog/phpdoc](https://phpdoc.daniil.it)