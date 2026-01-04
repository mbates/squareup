[**@bates-solutions/squareup API Reference v0.1.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [react](../README.md) / CreateOrderInput

# Interface: CreateOrderInput

Defined in: [src/react/hooks/useOrders.ts:23](https://github.com/mbates/squareup/blob/2891fe62b0e8af94ea47a5cdb6c79b3053a9ae62/src/react/hooks/useOrders.ts#L23)

Order creation options

## Properties

### customerId?

> `optional` **customerId**: `string`

Defined in: [src/react/hooks/useOrders.ts:27](https://github.com/mbates/squareup/blob/2891fe62b0e8af94ea47a5cdb6c79b3053a9ae62/src/react/hooks/useOrders.ts#L27)

Customer ID to associate with order

***

### lineItems

> **lineItems**: [`OrderLineItemInput`](OrderLineItemInput.md)[]

Defined in: [src/react/hooks/useOrders.ts:25](https://github.com/mbates/squareup/blob/2891fe62b0e8af94ea47a5cdb6c79b3053a9ae62/src/react/hooks/useOrders.ts#L25)

Line items for the order

***

### paymentToken?

> `optional` **paymentToken**: `string`

Defined in: [src/react/hooks/useOrders.ts:31](https://github.com/mbates/squareup/blob/2891fe62b0e8af94ea47a5cdb6c79b3053a9ae62/src/react/hooks/useOrders.ts#L31)

Optional payment token to pay for the order

***

### referenceId?

> `optional` **referenceId**: `string`

Defined in: [src/react/hooks/useOrders.ts:29](https://github.com/mbates/squareup/blob/2891fe62b0e8af94ea47a5cdb6c79b3053a9ae62/src/react/hooks/useOrders.ts#L29)

Reference ID for external tracking
