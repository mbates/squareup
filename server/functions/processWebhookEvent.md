[**@bates-solutions/squareup API Reference v1.9.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / processWebhookEvent

# Function: processWebhookEvent()

> **processWebhookEvent**(`event`, `config`): `Promise`\<`void`\>

Defined in: [server/webhook.ts:172](https://github.com/mbates/squareup/blob/756b613095b0aa87133212b3424e6f9269f64dfc/src/server/webhook.ts#L172)

Process a webhook event by calling the appropriate handler

## Parameters

### event

[`WebhookEvent`](../interfaces/WebhookEvent.md)

The parsed webhook event

### config

[`WebhookConfig`](../interfaces/WebhookConfig.md)

Webhook configuration with handlers

## Returns

`Promise`\<`void`\>

Promise that resolves when handler completes

## Example

```typescript
await processWebhookEvent(event, {
  signatureKey: process.env.SQUARE_WEBHOOK_KEY!,
  handlers: {
    'payment.created': async (event) => {
      console.log('Payment created:', event.data.id);
    },
  },
});
```
