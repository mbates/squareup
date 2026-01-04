[**@bates/squareup API Reference v0.1.0**](../../README.md)

***

[@bates/squareup API Reference](../../README.md) / [core](../README.md) / SquareClientConfig

# Interface: SquareClientConfig

Defined in: [src/core/client.ts:15](https://github.com/mbates/squareup/blob/5cbceb7be75e480372e4059c7badcdbbc730e2e4/src/core/client.ts#L15)

Configuration options for the Square client

## Properties

### accessToken

> **accessToken**: `string`

Defined in: [src/core/client.ts:19](https://github.com/mbates/squareup/blob/5cbceb7be75e480372e4059c7badcdbbc730e2e4/src/core/client.ts#L19)

Square API access token

***

### defaultCurrency?

> `optional` **defaultCurrency**: `string`

Defined in: [src/core/client.ts:36](https://github.com/mbates/squareup/blob/5cbceb7be75e480372e4059c7badcdbbc730e2e4/src/core/client.ts#L36)

Default currency code

#### Default

```ts
'USD'
```

***

### environment?

> `optional` **environment**: [`SquareEnvironment`](../type-aliases/SquareEnvironment.md)

Defined in: [src/core/client.ts:25](https://github.com/mbates/squareup/blob/5cbceb7be75e480372e4059c7badcdbbc730e2e4/src/core/client.ts#L25)

Square environment (sandbox or production)

#### Default

```ts
'sandbox'
```

***

### locationId?

> `optional` **locationId**: `string`

Defined in: [src/core/client.ts:30](https://github.com/mbates/squareup/blob/5cbceb7be75e480372e4059c7badcdbbc730e2e4/src/core/client.ts#L30)

Default location ID for operations that require it
