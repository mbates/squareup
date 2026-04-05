[**@bates-solutions/squareup API Reference v1.5.2**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / CatalogEventType

# Type Alias: CatalogEventType

> **CatalogEventType** = `"catalog.version.updated"`

Defined in: [server/types.ts:44](https://github.com/mbates/squareup/blob/6d0f048fcda3a2f66001b3d1fa98587fb99af062/src/server/types.ts#L44)

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
