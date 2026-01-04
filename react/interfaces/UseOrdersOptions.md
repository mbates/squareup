[**@bates/squareup API Reference v0.1.0**](../../README.md)

***

[@bates/squareup API Reference](../../README.md) / [react](../README.md) / UseOrdersOptions

# Interface: UseOrdersOptions

Defined in: [src/react/hooks/useOrders.ts:61](https://github.com/mbates/squareup/blob/5cbceb7be75e480372e4059c7badcdbbc730e2e4/src/react/hooks/useOrders.ts#L61)

Options for useOrders hook

## Properties

### apiEndpoint?

> `optional` **apiEndpoint**: `string`

Defined in: [src/react/hooks/useOrders.ts:63](https://github.com/mbates/squareup/blob/5cbceb7be75e480372e4059c7badcdbbc730e2e4/src/react/hooks/useOrders.ts#L63)

API endpoint for orders (default: /api/orders)

***

### onError()?

> `optional` **onError**: (`error`) => `void`

Defined in: [src/react/hooks/useOrders.ts:67](https://github.com/mbates/squareup/blob/5cbceb7be75e480372e4059c7badcdbbc730e2e4/src/react/hooks/useOrders.ts#L67)

Callback on order error

#### Parameters

##### error

`Error`

#### Returns

`void`

***

### onSuccess()?

> `optional` **onSuccess**: (`order`) => `void`

Defined in: [src/react/hooks/useOrders.ts:65](https://github.com/mbates/squareup/blob/5cbceb7be75e480372e4059c7badcdbbc730e2e4/src/react/hooks/useOrders.ts#L65)

Callback on successful order creation

#### Parameters

##### order

[`OrderResponse`](OrderResponse.md)

#### Returns

`void`
