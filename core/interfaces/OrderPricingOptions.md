[**@bates-solutions/squareup API Reference v1.12.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / OrderPricingOptions

# Interface: OrderPricingOptions

Defined in: [core/types/index.ts:80](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/types/index.ts#L80)

Pricing options for an order. Controls automatic application of discounts
(pricing rules) and taxes.

## Properties

### autoApplyDiscounts?

> `optional` **autoApplyDiscounts?**: `boolean`

Defined in: [core/types/index.ts:86](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/types/index.ts#L86)

Apply catalog pricing rules (incl. customer-group-gated wholesale rules)
automatically at calculation time. Required for order templates that back
subscriptions with per-retailer wholesale pricing.

***

### autoApplyTaxes?

> `optional` **autoApplyTaxes?**: `boolean`

Defined in: [core/types/index.ts:90](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/types/index.ts#L90)

Apply all enabled taxes at the location automatically.
