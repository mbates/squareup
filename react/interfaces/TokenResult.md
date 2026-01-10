[**@bates-solutions/squareup API Reference v0.2.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [react](../README.md) / TokenResult

# Interface: TokenResult

Defined in: [src/react/types.ts:125](https://github.com/mbates/squareup/blob/e1717f4e682df14ec77f74c91b6d5513106fd4d4/src/react/types.ts#L125)

## Properties

### details?

> `optional` **details**: `object`

Defined in: [src/react/types.ts:129](https://github.com/mbates/squareup/blob/e1717f4e682df14ec77f74c91b6d5513106fd4d4/src/react/types.ts#L129)

#### billing?

> `optional` **billing**: `object`

##### billing.postalCode?

> `optional` **postalCode**: `string`

#### card?

> `optional` **card**: `object`

##### card.brand

> **brand**: `string`

##### card.expMonth

> **expMonth**: `number`

##### card.expYear

> **expYear**: `number`

##### card.lastFour

> **lastFour**: `string`

#### method?

> `optional` **method**: `"Card"` \| `"GooglePay"` \| `"ApplePay"` \| `"GiftCard"` \| `"Ach"`

***

### errors?

> `optional` **errors**: [`TokenError`](TokenError.md)[]

Defined in: [src/react/types.ts:128](https://github.com/mbates/squareup/blob/e1717f4e682df14ec77f74c91b6d5513106fd4d4/src/react/types.ts#L128)

***

### status

> **status**: `"OK"` \| `"Cancel"` \| `"Error"`

Defined in: [src/react/types.ts:126](https://github.com/mbates/squareup/blob/e1717f4e682df14ec77f74c91b6d5513106fd4d4/src/react/types.ts#L126)

***

### token?

> `optional` **token**: `string`

Defined in: [src/react/types.ts:127](https://github.com/mbates/squareup/blob/e1717f4e682df14ec77f74c91b6d5513106fd4d4/src/react/types.ts#L127)
