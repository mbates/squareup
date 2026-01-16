[**@bates-solutions/squareup API Reference v1.1.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / SquareClientConfig

# Interface: SquareClientConfig

Defined in: [core/client.ts:16](https://github.com/mbates/squareup/blob/dbcba9ef6bec3f860a4170a9374bb001913ef9a5/src/core/client.ts#L16)

Configuration options for the Square client

## Properties

### accessToken

> **accessToken**: `string`

Defined in: [core/client.ts:20](https://github.com/mbates/squareup/blob/dbcba9ef6bec3f860a4170a9374bb001913ef9a5/src/core/client.ts#L20)

Square API access token

***

### defaultCurrency?

> `optional` **defaultCurrency**: `string`

Defined in: [core/client.ts:37](https://github.com/mbates/squareup/blob/dbcba9ef6bec3f860a4170a9374bb001913ef9a5/src/core/client.ts#L37)

Default currency code

#### Default

```ts
'USD'
```

***

### environment?

> `optional` **environment**: [`SquareEnvironment`](../type-aliases/SquareEnvironment.md)

Defined in: [core/client.ts:26](https://github.com/mbates/squareup/blob/dbcba9ef6bec3f860a4170a9374bb001913ef9a5/src/core/client.ts#L26)

Square environment (sandbox or production)

#### Default

```ts
'sandbox'
```

***

### locationId?

> `optional` **locationId**: `string`

Defined in: [core/client.ts:31](https://github.com/mbates/squareup/blob/dbcba9ef6bec3f860a4170a9374bb001913ef9a5/src/core/client.ts#L31)

Default location ID for operations that require it
