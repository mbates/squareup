[**@bates/squareup API Reference v0.1.0**](../../README.md)

***

[@bates/squareup API Reference](../../README.md) / [core](../README.md) / createSquareClient

# Function: createSquareClient()

> **createSquareClient**(`config`): [`SquareClient`](../classes/SquareClient.md)

Defined in: [src/core/client.ts:136](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/core/client.ts#L136)

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
