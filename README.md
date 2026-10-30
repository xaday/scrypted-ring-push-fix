# Scrypted Ring Push Fix

Unofficial community fix for Ring push notification decryption errors in Scrypted.

## Problem

Ring doorbell events may stop reaching Apple HomeKit due to:

ERR_CRYPTO_ECDH_INVALID_PUBLIC_KEY

## Tested solution

- Scrypted Ring Plugin: 0.0.146-ringfix.1
- Scrypted Server: 0.147.0
- @eneris/push-receiver: 4.3.1
- Scrypted source: v0.145.0
- Docker inside Proxmox LXC

## Results

Successfully tested with two Ring doorbells.

Both doorbells now trigger HomePod announcements through Apple HomeKit.

## Source and credits

Based on the community patch discussed in:
https://github.com/koush/scrypted/issues/2177

Scrypted:
https://github.com/koush/scrypted

Ring Client API:
https://github.com/koush/ring

## Distribution

This repository currently provides documentation of a tested community build.

The compiled plugin is not redistributed here pending clarification of the applicable licensing terms.

## Disclaimer

Unofficial community project. Not affiliated with or endorsed by the Scrypted maintainers.

Compatibility with other installations has not been verified.
