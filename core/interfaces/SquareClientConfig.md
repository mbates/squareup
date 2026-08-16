[**@bates-solutions/squareup API Reference v1.14.2**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / SquareClientConfig

# Interface: SquareClientConfig

Defined in: [core/client.ts:20](https://github.com/mbates/squareup/blob/a11d73be94c41c40737dd6a6343798e7b8db84de/src/core/client.ts#L20)

Configuration options for the Square client

## Properties

### accessToken

> **accessToken**: `string`

Defined in: [core/client.ts:24](https://github.com/mbates/squareup/blob/a11d73be94c41c40737dd6a6343798e7b8db84de/src/core/client.ts#L24)

Square API access token

***

### defaultCurrency?

> `optional` **defaultCurrency?**: `string`

Defined in: [core/client.ts:41](https://github.com/mbates/squareup/blob/a11d73be94c41c40737dd6a6343798e7b8db84de/src/core/client.ts#L41)

Default currency code

#### Default

```ts
'USD'
```

***

### environment?

> `optional` **environment?**: [`SquareEnvironment`](../type-aliases/SquareEnvironment.md)

Defined in: [core/client.ts:30](https://github.com/mbates/squareup/blob/a11d73be94c41c40737dd6a6343798e7b8db84de/src/core/client.ts#L30)

Square environment (sandbox or production)

#### Default

```ts
'sandbox'
```

***

### locationId?

> `optional` **locationId?**: `string`

Defined in: [core/client.ts:35](https://github.com/mbates/squareup/blob/a11d73be94c41c40737dd6a6343798e7b8db84de/src/core/client.ts#L35)

Default location ID for operations that require it
