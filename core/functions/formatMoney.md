[**@bates-solutions/squareup API Reference v0.2.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / formatMoney

# Function: formatMoney()

> **formatMoney**(`cents`, `currency`, `locale`): `string`

Defined in: [src/core/utils.ts:79](https://github.com/mbates/squareup/blob/e1717f4e682df14ec77f74c91b6d5513106fd4d4/src/core/utils.ts#L79)

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
