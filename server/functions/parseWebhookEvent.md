[**@bates-solutions/squareup API Reference v1.6.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / parseWebhookEvent

# Function: parseWebhookEvent()

> **parseWebhookEvent**(`rawBody`): [`WebhookEvent`](../interfaces/WebhookEvent.md)

Defined in: [server/webhook.ts:105](https://github.com/mbates/squareup/blob/f660af842439736b0c20211f3401c1f0023d5b33/src/server/webhook.ts#L105)

Parse a webhook request body into a typed event

## Parameters

### rawBody

`string`

The raw request body string

## Returns

[`WebhookEvent`](../interfaces/WebhookEvent.md)

Parsed webhook event

## Throws

Error if parsing fails

## Example

```typescript
const event = parseWebhookEvent(rawBody);
console.log(event.type); // 'payment.completed'
```
