[**@bates-solutions/squareup API Reference v1.13.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / parseWebhookEvent

# Function: parseWebhookEvent()

> **parseWebhookEvent**(`rawBody`): [`WebhookEvent`](../interfaces/WebhookEvent.md)

Defined in: [server/webhook.ts:105](https://github.com/mbates/squareup/blob/36eeb9010838e6df2f59b359e89c69f57fcea7b6/src/server/webhook.ts#L105)

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
