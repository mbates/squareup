[**@bates/squareup API Reference v0.1.0**](../../README.md)

***

[@bates/squareup API Reference](../../README.md) / [server](../README.md) / InventoryEventType

# Type Alias: InventoryEventType

> **InventoryEventType** = `"inventory.count.updated"`

Defined in: [src/server/types.ts:47](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/server/types.ts#L47)

@bates/squareup/server

Server utilities for handling Square webhooks

## Examples

```typescript
// Next.js App Router
import { createNextWebhookHandler } from '@bates/squareup/server';

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
import { createExpressWebhookHandler } from '@bates/squareup/server';

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
