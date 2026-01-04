[**@bates-solutions/squareup API Reference v0.1.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / WebhookConfig

# Interface: WebhookConfig

Defined in: [src/server/types.ts:111](https://github.com/mbates/squareup/blob/51442cfe91df1809d815d2acb88b04112b6ed3da/src/server/types.ts#L111)

Configuration for webhook handling

## Extended by

- [`ExpressWebhookOptions`](ExpressWebhookOptions.md)

## Properties

### handlers

> **handlers**: [`WebhookHandlers`](../type-aliases/WebhookHandlers.md)

Defined in: [src/server/types.ts:115](https://github.com/mbates/squareup/blob/51442cfe91df1809d815d2acb88b04112b6ed3da/src/server/types.ts#L115)

Event handlers by type

***

### notificationUrl?

> `optional` **notificationUrl**: `string`

Defined in: [src/server/types.ts:117](https://github.com/mbates/squareup/blob/51442cfe91df1809d815d2acb88b04112b6ed3da/src/server/types.ts#L117)

URL where webhooks are received (for signature verification)

***

### signatureKey

> **signatureKey**: `string`

Defined in: [src/server/types.ts:113](https://github.com/mbates/squareup/blob/51442cfe91df1809d815d2acb88b04112b6ed3da/src/server/types.ts#L113)

Square webhook signature key

***

### throwOnInvalidSignature?

> `optional` **throwOnInvalidSignature**: `boolean`

Defined in: [src/server/types.ts:122](https://github.com/mbates/squareup/blob/51442cfe91df1809d815d2acb88b04112b6ed3da/src/server/types.ts#L122)

Whether to throw on signature verification failure

#### Default

```ts
true
```
