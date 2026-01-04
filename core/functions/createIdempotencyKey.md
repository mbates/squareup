[**@bates/squareup API Reference v0.1.0**](../../README.md)

***

[@bates/squareup API Reference](../../README.md) / [core](../README.md) / createIdempotencyKey

# Function: createIdempotencyKey()

> **createIdempotencyKey**(): `string`

Defined in: [src/core/utils.ts:102](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/core/utils.ts#L102)

Create a unique idempotency key for Square API requests

## Returns

`string`

UUID string

## Example

```typescript
const key = createIdempotencyKey();
// "550e8400-e29b-41d4-a716-446655440000"
```
