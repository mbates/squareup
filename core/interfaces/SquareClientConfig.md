[**@bates-solutions/squareup API Reference v1.2.1**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / SquareClientConfig

# Interface: SquareClientConfig

Defined in: [core/client.ts:16](https://github.com/mbates/squareup/blob/63589cfc34c560e1faab8834479e5c143d24c255/src/core/client.ts#L16)

Configuration options for the Square client

## Properties

### accessToken

> **accessToken**: `string`

Defined in: [core/client.ts:20](https://github.com/mbates/squareup/blob/63589cfc34c560e1faab8834479e5c143d24c255/src/core/client.ts#L20)

Square API access token

***

### defaultCurrency?

> `optional` **defaultCurrency**: `string`

Defined in: [core/client.ts:37](https://github.com/mbates/squareup/blob/63589cfc34c560e1faab8834479e5c143d24c255/src/core/client.ts#L37)

Default currency code

#### Default

```ts
'USD'
```

***

### environment?

> `optional` **environment**: [`SquareEnvironment`](../type-aliases/SquareEnvironment.md)

Defined in: [core/client.ts:26](https://github.com/mbates/squareup/blob/63589cfc34c560e1faab8834479e5c143d24c255/src/core/client.ts#L26)

Square environment (sandbox or production)

#### Default

```ts
'sandbox'
```

***

### locationId?

> `optional` **locationId**: `string`

Defined in: [core/client.ts:31](https://github.com/mbates/squareup/blob/63589cfc34c560e1faab8834479e5c143d24c255/src/core/client.ts#L31)

Default location ID for operations that require it
