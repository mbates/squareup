[**@bates-solutions/squareup API Reference v1.14.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / formatMoney

# Function: formatMoney()

> **formatMoney**(`cents`, `currency?`, `locale?`): `string`

Defined in: [core/utils.ts:79](https://github.com/mbates/squareup/blob/449713f7707f00c7f34a87a330a88fd0868782c8/src/core/utils.ts#L79)

Format money for display

## Parameters

### cents

`number` \| `bigint`

Amount in smallest currency unit

### currency?

[`CurrencyCode`](../type-aliases/CurrencyCode.md) = `'USD'`

Currency code (default: USD)

### locale?

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
