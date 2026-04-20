[**@bates-solutions/squareup API Reference v1.12.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / LineItemInput

# Interface: LineItemInput

Defined in: [core/types/index.ts:44](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/types/index.ts#L44)

Line item for orders

## Properties

### amount?

> `optional` **amount?**: `number`

Defined in: [core/types/index.ts:48](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/types/index.ts#L48)

***

### basePriceMoney?

> `optional` **basePriceMoney?**: `object`

Defined in: [core/types/index.ts:54](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/types/index.ts#L54)

Explicit money override. When set, takes precedence over `amount` + the
builder's default currency. Useful for order templates where the base
price must include an explicit currency.

#### amount

> **amount**: `number` \| `bigint`

#### currency

> **currency**: [`CurrencyCode`](../type-aliases/CurrencyCode.md)

***

### catalogObjectId?

> `optional` **catalogObjectId?**: `string`

Defined in: [core/types/index.ts:46](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/types/index.ts#L46)

***

### name?

> `optional` **name?**: `string`

Defined in: [core/types/index.ts:45](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/types/index.ts#L45)

***

### note?

> `optional` **note?**: `string`

Defined in: [core/types/index.ts:58](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/types/index.ts#L58)

***

### quantity?

> `optional` **quantity?**: `number`

Defined in: [core/types/index.ts:47](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/types/index.ts#L47)
