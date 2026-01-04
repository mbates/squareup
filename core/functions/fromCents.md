[**@bates-solutions/squareup API Reference v0.1.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / fromCents

# Function: fromCents()

> **fromCents**(`cents`, `currency`): `number`

Defined in: [src/core/utils.ts:58](https://github.com/mbates/squareup/blob/51442cfe91df1809d815d2acb88b04112b6ed3da/src/core/utils.ts#L58)

Convert cents (smallest currency unit) to dollar amount

## Parameters

### cents

Amount in smallest currency unit

`number` | `bigint`

### currency

[`CurrencyCode`](../type-aliases/CurrencyCode.md) = `'USD'`

Currency code (default: USD)

## Returns

`number`

Dollar amount

## Example

```typescript
fromCents(1050n) // 10.50
fromCents(1050n, 'USD') // 10.50
fromCents(1000n, 'JPY') // 1000
```
