[**@bates-solutions/squareup API Reference v1.2.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / parseWebhookEvent

# Function: parseWebhookEvent()

> **parseWebhookEvent**(`rawBody`): [`WebhookEvent`](../interfaces/WebhookEvent.md)

Defined in: [server/webhook.ts:103](https://github.com/mbates/squareup/blob/2b85acb716e1cd46e6c182537b6d98fbcae0ef0b/src/server/webhook.ts#L103)

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
