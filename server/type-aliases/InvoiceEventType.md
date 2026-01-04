[**@bates-solutions/squareup API Reference v0.1.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / InvoiceEventType

# Type Alias: InvoiceEventType

> **InvoiceEventType** = `"invoice.created"` \| `"invoice.updated"` \| `"invoice.published"` \| `"invoice.payment_made"` \| `"invoice.canceled"`

Defined in: [src/server/types.ts:29](https://github.com/mbates/squareup/blob/51442cfe91df1809d815d2acb88b04112b6ed3da/src/server/types.ts#L29)

@bates-solutions/squareup/server

Server utilities for handling Square webhooks

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
