[**@bates-solutions/squareup API Reference v0.2.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / createIdempotencyKey

# Function: createIdempotencyKey()

> **createIdempotencyKey**(): `string`

Defined in: [src/core/utils.ts:102](https://github.com/mbates/squareup/blob/e1717f4e682df14ec77f74c91b6d5513106fd4d4/src/core/utils.ts#L102)

Create a unique idempotency key for Square API requests

## Returns

`string`

UUID string

## Example

```typescript
const key = createIdempotencyKey();
// "550e8400-e29b-41d4-a716-446655440000"
```
