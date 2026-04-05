[**@bates-solutions/squareup API Reference v1.6.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / OrderWebhookEvent

# Type Alias: OrderWebhookEvent

> **OrderWebhookEvent** = [`WebhookEvent`](../interfaces/WebhookEvent.md)\<[`OrderWebhookObject`](../interfaces/OrderWebhookObject.md)\> & `object`

Defined in: [server/types.ts:209](https://github.com/mbates/squareup/blob/f660af842439736b0c20211f3401c1f0023d5b33/src/server/types.ts#L209)

@bates-solutions/squareup/server

Server utilities for handling Square webhooks

## Type Declaration

### type

> **type**: [`OrderEventType`](OrderEventType.md)

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
