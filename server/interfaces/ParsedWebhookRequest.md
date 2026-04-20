[**@bates-solutions/squareup API Reference v1.12.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / ParsedWebhookRequest

# Interface: ParsedWebhookRequest

Defined in: [server/types.ts:138](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/server/types.ts#L138)

Parsed webhook request

## Properties

### event

> **event**: [`WebhookEvent`](WebhookEvent.md)

Defined in: [server/types.ts:144](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/server/types.ts#L144)

Parsed event data

***

### rawBody

> **rawBody**: `string`

Defined in: [server/types.ts:140](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/server/types.ts#L140)

The raw request body

***

### signature

> **signature**: `string`

Defined in: [server/types.ts:142](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/server/types.ts#L142)

The signature from headers
