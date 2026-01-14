[**@bates-solutions/squareup API Reference v1.0.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / createWebhookProcessor

# Function: createWebhookProcessor()

> **createWebhookProcessor**(`config`): (`rawBody`, `signature`) => `Promise`\<\{ `error?`: `string`; `event?`: [`WebhookEvent`](../interfaces/WebhookEvent.md)\<`unknown`\>; `success`: `boolean`; \}\>

Defined in: [server/webhook.ts:205](https://github.com/mbates/squareup/blob/32b2a6cc46d36384f60a869a504a33fd25157827/src/server/webhook.ts#L205)

Create a webhook handler function that verifies and processes events

## Parameters

### config

[`WebhookConfig`](../interfaces/WebhookConfig.md)

Webhook configuration

## Returns

Handler function that processes raw webhook requests

> (`rawBody`, `signature`): `Promise`\<\{ `error?`: `string`; `event?`: [`WebhookEvent`](../interfaces/WebhookEvent.md)\<`unknown`\>; `success`: `boolean`; \}\>

### Parameters

#### rawBody

`string`

#### signature

`string`

### Returns

`Promise`\<\{ `error?`: `string`; `event?`: [`WebhookEvent`](../interfaces/WebhookEvent.md)\<`unknown`\>; `success`: `boolean`; \}\>

## Example

```typescript
const handleWebhook = createWebhookProcessor({
  signatureKey: process.env.SQUARE_WEBHOOK_KEY!,
  handlers: {
    'payment.created': async (event) => {
      await sendReceipt(event.data.object.payment);
    },
    'order.updated': async (event) => {
      await updateOrderStatus(event.data.object.order);
    },
  },
});

// Use in your route handler
const result = await handleWebhook(rawBody, signature);
```
