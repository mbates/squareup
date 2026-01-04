[**@bates/squareup API Reference v0.1.0**](../../README.md)

***

[@bates/squareup API Reference](../../README.md) / [core](../README.md) / formatMoney

# Function: formatMoney()

> **formatMoney**(`cents`, `currency`, `locale`): `string`

Defined in: [src/core/utils.ts:79](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/core/utils.ts#L79)

Format money for display

## Parameters

### cents

Amount in smallest currency unit

`number` | `bigint`

### currency

[`CurrencyCode`](../type-aliases/CurrencyCode.md) = `'USD'`

Currency code (default: USD)

### locale

`string` = `'en-US'`

Locale for formatting (default: en-US)

## Returns

`string`

Formatted currency string

## Example

```typescript
formatMoney(1050n) // "$10.50"
formatMoney(1050n, 'USD', 'en-US') // "$10.50"
formatMoney(1000n, 'JPY', 'ja-JP') // "¥1,000"
```
