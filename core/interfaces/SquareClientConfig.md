[**@bates-solutions/squareup API Reference v1.9.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / SquareClientConfig

# Interface: SquareClientConfig

Defined in: [core/client.ts:17](https://github.com/mbates/squareup/blob/756b613095b0aa87133212b3424e6f9269f64dfc/src/core/client.ts#L17)

Configuration options for the Square client

## Properties

### accessToken

> **accessToken**: `string`

Defined in: [core/client.ts:21](https://github.com/mbates/squareup/blob/756b613095b0aa87133212b3424e6f9269f64dfc/src/core/client.ts#L21)

Square API access token

***

### defaultCurrency?

> `optional` **defaultCurrency?**: `string`

Defined in: [core/client.ts:38](https://github.com/mbates/squareup/blob/756b613095b0aa87133212b3424e6f9269f64dfc/src/core/client.ts#L38)

Default currency code

#### Default

```ts
'USD'
```

***

### environment?

> `optional` **environment?**: [`SquareEnvironment`](../type-aliases/SquareEnvironment.md)

Defined in: [core/client.ts:27](https://github.com/mbates/squareup/blob/756b613095b0aa87133212b3424e6f9269f64dfc/src/core/client.ts#L27)

Square environment (sandbox or production)

#### Default

```ts
'sandbox'
```

***

### locationId?

> `optional` **locationId?**: `string`

Defined in: [core/client.ts:32](https://github.com/mbates/squareup/blob/756b613095b0aa87133212b3424e6f9269f64dfc/src/core/client.ts#L32)

Default location ID for operations that require it
