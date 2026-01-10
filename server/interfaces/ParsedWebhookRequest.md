[**@bates-solutions/squareup API Reference v0.2.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / ParsedWebhookRequest

# Interface: ParsedWebhookRequest

Defined in: [src/server/types.ts:138](https://github.com/mbates/squareup/blob/8c46134cf39ac2cfc86b2d998f7cb56c9436089e/src/server/types.ts#L138)

Parsed webhook request

## Properties

### event

> **event**: [`WebhookEvent`](WebhookEvent.md)

Defined in: [src/server/types.ts:144](https://github.com/mbates/squareup/blob/8c46134cf39ac2cfc86b2d998f7cb56c9436089e/src/server/types.ts#L144)

Parsed event data

***

### rawBody

> **rawBody**: `string`

Defined in: [src/server/types.ts:140](https://github.com/mbates/squareup/blob/8c46134cf39ac2cfc86b2d998f7cb56c9436089e/src/server/types.ts#L140)

The raw request body

***

### signature

> **signature**: `string`

Defined in: [src/server/types.ts:142](https://github.com/mbates/squareup/blob/8c46134cf39ac2cfc86b2d998f7cb56c9436089e/src/server/types.ts#L142)

The signature from headers
