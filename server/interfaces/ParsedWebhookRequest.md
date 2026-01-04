[**@bates-solutions/squareup API Reference v0.1.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / ParsedWebhookRequest

# Interface: ParsedWebhookRequest

Defined in: [src/server/types.ts:138](https://github.com/mbates/squareup/blob/824f4816f17ba50f86315ee987746e0a114472bf/src/server/types.ts#L138)

Parsed webhook request

## Properties

### event

> **event**: [`WebhookEvent`](WebhookEvent.md)

Defined in: [src/server/types.ts:144](https://github.com/mbates/squareup/blob/824f4816f17ba50f86315ee987746e0a114472bf/src/server/types.ts#L144)

Parsed event data

***

### rawBody

> **rawBody**: `string`

Defined in: [src/server/types.ts:140](https://github.com/mbates/squareup/blob/824f4816f17ba50f86315ee987746e0a114472bf/src/server/types.ts#L140)

The raw request body

***

### signature

> **signature**: `string`

Defined in: [src/server/types.ts:142](https://github.com/mbates/squareup/blob/824f4816f17ba50f86315ee987746e0a114472bf/src/server/types.ts#L142)

The signature from headers
