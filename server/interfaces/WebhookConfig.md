[**@bates-solutions/squareup API Reference v1.13.2**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / WebhookConfig

# Interface: WebhookConfig

Defined in: [server/types.ts:111](https://github.com/mbates/squareup/blob/ef064123281909ad68ffbd0881a9f18aa0842e3a/src/server/types.ts#L111)

Configuration for webhook handling

## Extended by

- [`ExpressWebhookOptions`](ExpressWebhookOptions.md)

## Properties

### handlers

> **handlers**: [`WebhookHandlers`](../type-aliases/WebhookHandlers.md)

Defined in: [server/types.ts:115](https://github.com/mbates/squareup/blob/ef064123281909ad68ffbd0881a9f18aa0842e3a/src/server/types.ts#L115)

Event handlers by type

***

### notificationUrl?

> `optional` **notificationUrl?**: `string`

Defined in: [server/types.ts:117](https://github.com/mbates/squareup/blob/ef064123281909ad68ffbd0881a9f18aa0842e3a/src/server/types.ts#L117)

URL where webhooks are received (for signature verification)

***

### signatureKey

> **signatureKey**: `string`

Defined in: [server/types.ts:113](https://github.com/mbates/squareup/blob/ef064123281909ad68ffbd0881a9f18aa0842e3a/src/server/types.ts#L113)

Square webhook signature key

***

### throwOnInvalidSignature?

> `optional` **throwOnInvalidSignature?**: `boolean`

Defined in: [server/types.ts:122](https://github.com/mbates/squareup/blob/ef064123281909ad68ffbd0881a9f18aa0842e3a/src/server/types.ts#L122)

Whether to throw on signature verification failure

#### Default

```ts
true
```
