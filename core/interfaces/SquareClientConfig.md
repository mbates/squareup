[**@bates-solutions/squareup API Reference v1.13.2**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / SquareClientConfig

# Interface: SquareClientConfig

Defined in: [core/client.ts:18](https://github.com/mbates/squareup/blob/a3370a50f8aa881cfc5ad90f5282a919659930de/src/core/client.ts#L18)

Configuration options for the Square client

## Properties

### accessToken

> **accessToken**: `string`

Defined in: [core/client.ts:22](https://github.com/mbates/squareup/blob/a3370a50f8aa881cfc5ad90f5282a919659930de/src/core/client.ts#L22)

Square API access token

***

### defaultCurrency?

> `optional` **defaultCurrency?**: `string`

Defined in: [core/client.ts:39](https://github.com/mbates/squareup/blob/a3370a50f8aa881cfc5ad90f5282a919659930de/src/core/client.ts#L39)

Default currency code

#### Default

```ts
'USD'
```

***

### environment?

> `optional` **environment?**: [`SquareEnvironment`](../type-aliases/SquareEnvironment.md)

Defined in: [core/client.ts:28](https://github.com/mbates/squareup/blob/a3370a50f8aa881cfc5ad90f5282a919659930de/src/core/client.ts#L28)

Square environment (sandbox or production)

#### Default

```ts
'sandbox'
```

***

### locationId?

> `optional` **locationId?**: `string`

Defined in: [core/client.ts:33](https://github.com/mbates/squareup/blob/a3370a50f8aa881cfc5ad90f5282a919659930de/src/core/client.ts#L33)

Default location ID for operations that require it
