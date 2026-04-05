[**@bates-solutions/squareup API Reference v1.6.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / fromCents

# Function: fromCents()

> **fromCents**(`cents`, `currency?`): `number`

Defined in: [core/utils.ts:58](https://github.com/mbates/squareup/blob/f660af842439736b0c20211f3401c1f0023d5b33/src/core/utils.ts#L58)

Convert cents (smallest currency unit) to dollar amount

## Parameters

### cents

`number` \| `bigint`

Amount in smallest currency unit

### currency?

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
