[**@bates-solutions/squareup API Reference v1.10.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / RefundWebhookObject

# Interface: RefundWebhookObject

Defined in: [server/types.ts:180](https://github.com/mbates/squareup/blob/bd0cc77dd8a0653f0d66788f752f3f831d55e75c/src/server/types.ts#L180)

Refund object in a webhook event payload

## Properties

### refund

> **refund**: `object`

Defined in: [server/types.ts:181](https://github.com/mbates/squareup/blob/bd0cc77dd8a0653f0d66788f752f3f831d55e75c/src/server/types.ts#L181)

#### amount\_money?

> `optional` **amount\_money?**: `object`

##### amount\_money.amount

> **amount**: `number`

##### amount\_money.currency

> **currency**: `string`

#### id

> **id**: `string`

#### order\_id?

> `optional` **order\_id?**: `string`

#### payment\_id

> **payment\_id**: `string`

#### status

> **status**: `string`
