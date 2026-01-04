[**@bates-solutions/squareup API Reference v0.1.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / parseWebhookEvent

# Function: parseWebhookEvent()

> **parseWebhookEvent**(`rawBody`): [`WebhookEvent`](../interfaces/WebhookEvent.md)

Defined in: [src/server/webhook.ts:103](https://github.com/mbates/squareup/blob/2891fe62b0e8af94ea47a5cdb6c79b3053a9ae62/src/server/webhook.ts#L103)

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
