[**@bates-solutions/squareup API Reference v1.13.2**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / createNextWebhookHandler

# Function: createNextWebhookHandler()

> **createNextWebhookHandler**(`config`): (`request`) => `Promise`\<`Response`\>

Defined in: [server/middleware/nextjs.ts:66](https://github.com/mbates/squareup/blob/ef064123281909ad68ffbd0881a9f18aa0842e3a/src/server/middleware/nextjs.ts#L66)

Create a Next.js App Router webhook handler

## Parameters

### config

[`WebhookConfig`](../interfaces/WebhookConfig.md)

Webhook configuration

## Returns

Route handler for POST requests

(`request`) => `Promise`\<`Response`\>

## Example

```typescript
// app/api/webhook/route.ts
import { createNextWebhookHandler } from '@bates-solutions/squareup/server';

export const POST = createNextWebhookHandler({
  signatureKey: process.env.SQUARE_WEBHOOK_KEY!,
  handlers: {
    'payment.created': async (event) => {
      console.log('Payment created:', event.data.id);
    },
    'order.fulfillment.updated': async (event) => {
      await notifyCustomer(event.data.object);
    },
  },
});
```
