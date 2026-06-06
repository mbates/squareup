[**@bates-solutions/squareup API Reference v1.13.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / GiftCardState

# Type Alias: GiftCardState

> **GiftCardState** = `"PENDING"` \| `"ACTIVE"` \| `"DEACTIVATED"` \| `"BLOCKED"` \| `"UNLINKED_OWNER"`

Defined in: [core/services/gift-cards.service.ts:25](https://github.com/mbates/squareup/blob/36eeb9010838e6df2f59b359e89c69f57fcea7b6/src/core/services/gift-cards.service.ts#L25)

Lifecycle state of a gift card.

New cards start in `PENDING` and require an `ACTIVATE` activity before they
can be redeemed.
