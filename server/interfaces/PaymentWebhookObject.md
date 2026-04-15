[**@bates-solutions/squareup API Reference v1.10.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / PaymentWebhookObject

# Interface: PaymentWebhookObject

Defined in: [server/types.ts:152](https://github.com/mbates/squareup/blob/f92173636cb82aa5c787e6b2748fad54d675bfbf/src/server/types.ts#L152)

Payment object in a webhook event payload

## Properties

### payment

> **payment**: `object`

Defined in: [server/types.ts:153](https://github.com/mbates/squareup/blob/f92173636cb82aa5c787e6b2748fad54d675bfbf/src/server/types.ts#L153)

#### amount\_money?

> `optional` **amount\_money?**: `object`

##### amount\_money.amount

> **amount**: `number`

##### amount\_money.currency

> **currency**: `string`

#### created\_at?

> `optional` **created\_at?**: `string`

#### customer\_id?

> `optional` **customer\_id?**: `string`

#### id

> **id**: `string`

#### location\_id?

> `optional` **location\_id?**: `string`

#### order\_id?

> `optional` **order\_id?**: `string`

#### source\_type?

> `optional` **source\_type?**: `string`

#### status

> **status**: `string`

#### updated\_at?

> `optional` **updated\_at?**: `string`
