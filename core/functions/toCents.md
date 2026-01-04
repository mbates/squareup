[**@bates/squareup API Reference v0.1.0**](../../README.md)

***

[@bates/squareup API Reference](../../README.md) / [core](../README.md) / toCents

# Function: toCents()

> **toCents**(`amount`, `currency`): `bigint`

Defined in: [src/core/utils.ts:38](https://github.com/mbates/squareup/blob/5cbceb7be75e480372e4059c7badcdbbc730e2e4/src/core/utils.ts#L38)

Convert a dollar amount to cents (smallest currency unit)

## Parameters

### amount

`number`

Dollar amount (e.g., 10.50)

### currency

[`CurrencyCode`](../type-aliases/CurrencyCode.md) = `'USD'`

Currency code (default: USD)

## Returns

`bigint`

Amount in smallest currency unit (e.g., 1050 for $10.50 USD)

## Example

```typescript
toCents(10.50) // 1050
toCents(10.50, 'USD') // 1050
toCents(1000, 'JPY') // 1000 (JPY has no decimal places)
```
