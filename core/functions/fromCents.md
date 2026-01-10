[**@bates-solutions/squareup API Reference v0.2.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / fromCents

# Function: fromCents()

> **fromCents**(`cents`, `currency`): `number`

Defined in: [src/core/utils.ts:58](https://github.com/mbates/squareup/blob/d6b2fac41166e6715afbe2a8bcbab0c784e759f8/src/core/utils.ts#L58)

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
