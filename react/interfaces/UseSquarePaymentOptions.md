[**@bates/squareup API Reference v0.1.0**](../../README.md)

***

[@bates/squareup API Reference](../../README.md) / [react](../README.md) / UseSquarePaymentOptions

# Interface: UseSquarePaymentOptions

Defined in: [src/react/hooks/useSquarePayment.ts:8](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/react/hooks/useSquarePayment.ts#L8)

Options for useSquarePayment hook

## Properties

### cardOptions?

> `optional` **cardOptions**: [`CardOptions`](CardOptions.md)

Defined in: [src/react/hooks/useSquarePayment.ts:10](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/react/hooks/useSquarePayment.ts#L10)

Card input styling options

***

### onError()?

> `optional` **onError**: (`error`) => `void`

Defined in: [src/react/hooks/useSquarePayment.ts:16](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/react/hooks/useSquarePayment.ts#L16)

Callback when an error occurs

#### Parameters

##### error

`Error`

#### Returns

`void`

***

### onReady()?

> `optional` **onReady**: () => `void`

Defined in: [src/react/hooks/useSquarePayment.ts:12](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/react/hooks/useSquarePayment.ts#L12)

Callback when card is ready

#### Returns

`void`

***

### onTokenize()?

> `optional` **onTokenize**: (`token`) => `void`

Defined in: [src/react/hooks/useSquarePayment.ts:14](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/react/hooks/useSquarePayment.ts#L14)

Callback when tokenization succeeds

#### Parameters

##### token

`string`

#### Returns

`void`
