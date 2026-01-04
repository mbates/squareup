[**@bates-solutions/squareup API Reference v0.1.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [react](../README.md) / UsePaymentsOptions

# Interface: UsePaymentsOptions

Defined in: [src/react/hooks/usePayments.ts:45](https://github.com/mbates/squareup/blob/824f4816f17ba50f86315ee987746e0a114472bf/src/react/hooks/usePayments.ts#L45)

Options for usePayments hook

## Properties

### apiEndpoint?

> `optional` **apiEndpoint**: `string`

Defined in: [src/react/hooks/usePayments.ts:47](https://github.com/mbates/squareup/blob/824f4816f17ba50f86315ee987746e0a114472bf/src/react/hooks/usePayments.ts#L47)

API endpoint for creating payments (default: /api/payments)

***

### onError()?

> `optional` **onError**: (`error`) => `void`

Defined in: [src/react/hooks/usePayments.ts:51](https://github.com/mbates/squareup/blob/824f4816f17ba50f86315ee987746e0a114472bf/src/react/hooks/usePayments.ts#L51)

Callback on payment error

#### Parameters

##### error

`Error`

#### Returns

`void`

***

### onSuccess()?

> `optional` **onSuccess**: (`payment`) => `void`

Defined in: [src/react/hooks/usePayments.ts:49](https://github.com/mbates/squareup/blob/824f4816f17ba50f86315ee987746e0a114472bf/src/react/hooks/usePayments.ts#L49)

Callback on successful payment

#### Parameters

##### payment

[`PaymentResponse`](PaymentResponse.md)

#### Returns

`void`
