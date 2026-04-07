[**@bates-solutions/squareup API Reference v1.8.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / RefundWebhookEvent

# Type Alias: RefundWebhookEvent

> **RefundWebhookEvent** = [`WebhookEvent`](../interfaces/WebhookEvent.md)\<[`RefundWebhookObject`](../interfaces/RefundWebhookObject.md)\> & `object`

Defined in: [server/types.ts:212](https://github.com/mbates/squareup/blob/e8b175f9fa135da3fad7a826c83967bf8ac499a5/src/server/types.ts#L212)

@bates-solutions/squareup/server

Server utilities for handling Square webhooks

## Type Declaration

### type

> **type**: [`RefundEventType`](RefundEventType.md)

## Examples

```typescript
// Next.js App Router
import { createNextWebhookHandler } from '@bates-solutions/squareup/server';

export const POST = createNextWebhookHandler({
  signatureKey: process.env.SQUARE_WEBHOOK_KEY!,
  handlers: {
    'payment.created': async (event) => {
      console.log('Payment:', event.data.id);
    },
  },
});
```

```typescript
// Express
import express from 'express';
import { createExpressWebhookHandler } from '@bates-solutions/squareup/server';

const app = express();
app.use('/webhook', express.raw({ type: 'application/json' }));
app.post('/webhook', createExpressWebhookHandler({
  signatureKey: process.env.SQUARE_WEBHOOK_KEY!,
  handlers: {
    'payment.created': async (event) => {
      console.log('Payment:', event.data.id);
    },
  },
}));
```
