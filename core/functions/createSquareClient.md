[**@bates-solutions/squareup API Reference v1.4.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / createSquareClient

# Function: createSquareClient()

> **createSquareClient**(`config`): [`SquareClient`](../classes/SquareClient.md)

Defined in: [core/client.ts:139](https://github.com/mbates/squareup/blob/57c8fcd614ec400c089d1bd7914e78c796994d0e/src/core/client.ts#L139)

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
