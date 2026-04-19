[**@bates-solutions/squareup API Reference v1.10.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / createNextPagesWebhookHandler

# Function: createNextPagesWebhookHandler()

> **createNextPagesWebhookHandler**(`config`): (`req`, `res`) => `Promise`\<`void`\>

Defined in: [server/middleware/nextjs.ts:138](https://github.com/mbates/squareup/blob/bd0cc77dd8a0653f0d66788f752f3f831d55e75c/src/server/middleware/nextjs.ts#L138)

Create a Next.js Pages Router API handler

## Parameters

### config

[`WebhookConfig`](../interfaces/WebhookConfig.md)

Webhook configuration

## Returns

API route handler

(`req`, `res`) => `Promise`\<`void`\>

## Example

```typescript
// pages/api/webhook.ts
import { createNextPagesWebhookHandler } from '@bates-solutions/squareup/server';

export const config = {
  api: { bodyParser: false }, // Required for raw body
};

export default createNextPagesWebhookHandler({
  signatureKey: process.env.SQUARE_WEBHOOK_KEY!,
  handlers: {
    'payment.created': async (event) => {
      console.log('Payment:', event.data.id);
    },
  },
});
```
