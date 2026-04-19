[**@bates-solutions/squareup API Reference v1.10.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / CustomerWebhookEvent

# Type Alias: CustomerWebhookEvent

> **CustomerWebhookEvent** = [`WebhookEvent`](../interfaces/WebhookEvent.md)\<[`CustomerWebhookObject`](../interfaces/CustomerWebhookObject.md)\> & `object`

Defined in: [server/types.ts:215](https://github.com/mbates/squareup/blob/bd0cc77dd8a0653f0d66788f752f3f831d55e75c/src/server/types.ts#L215)

@bates-solutions/squareup/server

Server utilities for handling Square webhooks

## Type Declaration

### type

> **type**: [`CustomerEventType`](CustomerEventType.md)

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
