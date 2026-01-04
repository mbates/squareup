[**@bates/squareup API Reference v0.1.0**](../../README.md)

***

[@bates/squareup API Reference](../../README.md) / [server](../README.md) / parseNextWebhook

# Function: parseNextWebhook()

> **parseNextWebhook**(`request`, `signatureKey`, `notificationUrl?`): `Promise`\<[`WebhookEvent`](../interfaces/WebhookEvent.md)\<`unknown`\>\>

Defined in: [src/server/middleware/nextjs.ts:238](https://github.com/mbates/squareup/blob/5cbceb7be75e480372e4059c7badcdbbc730e2e4/src/server/middleware/nextjs.ts#L238)

Utility to parse webhook event from Next.js request

Use this for custom handling when you don't want automatic processing

## Parameters

### request

`Request`

The incoming request

### signatureKey

`string`

Your webhook signature key

### notificationUrl?

`string`

Optional URL for signature verification

## Returns

`Promise`\<[`WebhookEvent`](../interfaces/WebhookEvent.md)\<`unknown`\>\>

Parsed webhook event

## Throws

Error if verification fails

## Example

```typescript
// app/api/webhook/route.ts
import { parseNextWebhook } from '@bates/squareup/server';

export async function POST(request: Request) {
  const event = await parseNextWebhook(
    request,
    process.env.SQUARE_WEBHOOK_KEY!
  );

  // Custom handling
  switch (event.type) {
    case 'payment.created':
      // ...
  }

  return Response.json({ received: true });
}
```
