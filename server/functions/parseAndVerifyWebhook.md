[**@bates-solutions/squareup API Reference v0.2.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / parseAndVerifyWebhook

# Function: parseAndVerifyWebhook()

> **parseAndVerifyWebhook**(`rawBody`, `signature`, `signatureKey`, `notificationUrl?`): [`ParsedWebhookRequest`](../interfaces/ParsedWebhookRequest.md)

Defined in: [src/server/webhook.ts:130](https://github.com/mbates/squareup/blob/d6b2fac41166e6715afbe2a8bcbab0c784e759f8/src/server/webhook.ts#L130)

Parse and verify a webhook request

## Parameters

### rawBody

`string`

The raw request body string

### signature

`string`

The signature from headers

### signatureKey

`string`

Your webhook signature key

### notificationUrl?

`string`

Optional notification URL for verification

## Returns

[`ParsedWebhookRequest`](../interfaces/ParsedWebhookRequest.md)

Parsed and verified webhook request

## Throws

Error if verification or parsing fails

## Example

```typescript
const { event } = parseAndVerifyWebhook(
  rawBody,
  signature,
  process.env.SQUARE_WEBHOOK_KEY!
);
```
