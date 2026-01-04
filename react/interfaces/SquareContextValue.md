[**@bates/squareup API Reference v0.1.0**](../../README.md)

***

[@bates/squareup API Reference](../../README.md) / [react](../README.md) / SquareContextValue

# Interface: SquareContextValue

Defined in: [src/react/types.ts:22](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/react/types.ts#L22)

Square context value

## Properties

### config

> **config**: [`SquareProviderConfig`](SquareProviderConfig.md)

Defined in: [src/react/types.ts:24](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/react/types.ts#L24)

Configuration

***

### error

> **error**: `Error` \| `null`

Defined in: [src/react/types.ts:30](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/react/types.ts#L30)

Error if SDK failed to load

***

### payments

> **payments**: [`Payments`](Payments.md) \| `null`

Defined in: [src/react/types.ts:28](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/react/types.ts#L28)

Square Payments instance

***

### sdkLoaded

> **sdkLoaded**: `boolean`

Defined in: [src/react/types.ts:26](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/react/types.ts#L26)

Whether the Web Payments SDK is loaded
