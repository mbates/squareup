[**@bates-solutions/squareup API Reference v1.14.2**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / createSquareClient

# Function: createSquareClient()

> **createSquareClient**(`config`): [`SquareClient`](../classes/SquareClient.md)

Defined in: [core/client.ts:145](https://github.com/mbates/squareup/blob/e68db3ef52af57ddb49e3a70a5caa48fda64cc36/src/core/client.ts#L145)

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
