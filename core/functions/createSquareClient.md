[**@bates-solutions/squareup API Reference v1.1.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / createSquareClient

# Function: createSquareClient()

> **createSquareClient**(`config`): [`SquareClient`](../classes/SquareClient.md)

Defined in: [core/client.ts:139](https://github.com/mbates/squareup/blob/dbcba9ef6bec3f860a4170a9374bb001913ef9a5/src/core/client.ts#L139)

Create a new Square client instance

## Parameters

### config

[`SquareClientConfig`](../interfaces/SquareClientConfig.md)

Client configuration

## Returns

[`SquareClient`](../classes/SquareClient.md)

Configured Square client

## Example

```typescript
const square = createSquareClient({
  accessToken: process.env.SQUARE_ACCESS_TOKEN!,
  environment: 'sandbox',
});
```
