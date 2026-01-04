[**@bates-solutions/squareup API Reference v0.1.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [react](../README.md) / UseOrdersOptions

# Interface: UseOrdersOptions

Defined in: [src/react/hooks/useOrders.ts:61](https://github.com/mbates/squareup/blob/2891fe62b0e8af94ea47a5cdb6c79b3053a9ae62/src/react/hooks/useOrders.ts#L61)

Options for useOrders hook

## Properties

### apiEndpoint?

> `optional` **apiEndpoint**: `string`

Defined in: [src/react/hooks/useOrders.ts:63](https://github.com/mbates/squareup/blob/2891fe62b0e8af94ea47a5cdb6c79b3053a9ae62/src/react/hooks/useOrders.ts#L63)

API endpoint for orders (default: /api/orders)

***

### onError()?

> `optional` **onError**: (`error`) => `void`

Defined in: [src/react/hooks/useOrders.ts:67](https://github.com/mbates/squareup/blob/2891fe62b0e8af94ea47a5cdb6c79b3053a9ae62/src/react/hooks/useOrders.ts#L67)

Callback on order error

#### Parameters

##### error

`Error`

#### Returns

`void`

***

### onSuccess()?

> `optional` **onSuccess**: (`order`) => `void`

Defined in: [src/react/hooks/useOrders.ts:65](https://github.com/mbates/squareup/blob/2891fe62b0e8af94ea47a5cdb6c79b3053a9ae62/src/react/hooks/useOrders.ts#L65)

Callback on successful order creation

#### Parameters

##### order

[`OrderResponse`](OrderResponse.md)

#### Returns

`void`
