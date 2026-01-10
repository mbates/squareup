[**@bates-solutions/squareup API Reference v0.2.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / SquareClientConfig

# Interface: SquareClientConfig

Defined in: [core/client.ts:15](https://github.com/mbates/squareup/blob/7fc1f90acc9e8ec4ffc6c0b33c0e5d3803366ae1/src/core/client.ts#L15)

Configuration options for the Square client

## Properties

### accessToken

> **accessToken**: `string`

Defined in: [core/client.ts:19](https://github.com/mbates/squareup/blob/7fc1f90acc9e8ec4ffc6c0b33c0e5d3803366ae1/src/core/client.ts#L19)

Square API access token

***

### defaultCurrency?

> `optional` **defaultCurrency**: `string`

Defined in: [core/client.ts:36](https://github.com/mbates/squareup/blob/7fc1f90acc9e8ec4ffc6c0b33c0e5d3803366ae1/src/core/client.ts#L36)

Default currency code

#### Default

```ts
'USD'
```

***

### environment?

> `optional` **environment**: [`SquareEnvironment`](../type-aliases/SquareEnvironment.md)

Defined in: [core/client.ts:25](https://github.com/mbates/squareup/blob/7fc1f90acc9e8ec4ffc6c0b33c0e5d3803366ae1/src/core/client.ts#L25)

Square environment (sandbox or production)

#### Default

```ts
'sandbox'
```

***

### locationId?

> `optional` **locationId**: `string`

Defined in: [core/client.ts:30](https://github.com/mbates/squareup/blob/7fc1f90acc9e8ec4ffc6c0b33c0e5d3803366ae1/src/core/client.ts#L30)

Default location ID for operations that require it
