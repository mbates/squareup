[**@bates-solutions/squareup API Reference v1.13.1**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / GiftCardState

# Type Alias: GiftCardState

> **GiftCardState** = `"PENDING"` \| `"ACTIVE"` \| `"DEACTIVATED"` \| `"BLOCKED"` \| `"UNLINKED_OWNER"`

Defined in: [core/services/gift-cards.service.ts:25](https://github.com/mbates/squareup/blob/062721e435bb8ebf7b21ecf236e68c6a5f5432e7/src/core/services/gift-cards.service.ts#L25)

Lifecycle state of a gift card.

New cards start in `PENDING` and require an `ACTIVATE` activity before they
can be redeemed.
