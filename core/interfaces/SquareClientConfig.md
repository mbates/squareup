[**@bates-solutions/squareup API Reference v1.12.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / SquareClientConfig

# Interface: SquareClientConfig

Defined in: [core/client.ts:18](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/client.ts#L18)

Configuration options for the Square client

## Properties

### accessToken

> **accessToken**: `string`

Defined in: [core/client.ts:22](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/client.ts#L22)

Square API access token

***

### defaultCurrency?

> `optional` **defaultCurrency?**: `string`

Defined in: [core/client.ts:39](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/client.ts#L39)

Default currency code

#### Default

```ts
'USD'
```

***

### environment?

> `optional` **environment?**: [`SquareEnvironment`](../type-aliases/SquareEnvironment.md)

Defined in: [core/client.ts:28](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/client.ts#L28)

Square environment (sandbox or production)

#### Default

```ts
'sandbox'
```

***

### locationId?

> `optional` **locationId?**: `string`

Defined in: [core/client.ts:33](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/client.ts#L33)

Default location ID for operations that require it
