[**@bates-solutions/squareup API Reference v0.2.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / createIdempotencyKey

# Function: createIdempotencyKey()

> **createIdempotencyKey**(): `string`

Defined in: [src/core/utils.ts:102](https://github.com/mbates/squareup/blob/8c46134cf39ac2cfc86b2d998f7cb56c9436089e/src/core/utils.ts#L102)

Create a unique idempotency key for Square API requests

## Returns

`string`

UUID string

## Example

```typescript
const key = createIdempotencyKey();
// "550e8400-e29b-41d4-a716-446655440000"
```
