[**@bates-solutions/squareup API Reference v1.4.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / ParsedWebhookRequest

# Interface: ParsedWebhookRequest

Defined in: [server/types.ts:138](https://github.com/mbates/squareup/blob/57c8fcd614ec400c089d1bd7914e78c796994d0e/src/server/types.ts#L138)

Parsed webhook request

## Properties

### event

> **event**: [`WebhookEvent`](WebhookEvent.md)

Defined in: [server/types.ts:144](https://github.com/mbates/squareup/blob/57c8fcd614ec400c089d1bd7914e78c796994d0e/src/server/types.ts#L144)

Parsed event data

***

### rawBody

> **rawBody**: `string`

Defined in: [server/types.ts:140](https://github.com/mbates/squareup/blob/57c8fcd614ec400c089d1bd7914e78c796994d0e/src/server/types.ts#L140)

The raw request body

***

### signature

> **signature**: `string`

Defined in: [server/types.ts:142](https://github.com/mbates/squareup/blob/57c8fcd614ec400c089d1bd7914e78c796994d0e/src/server/types.ts#L142)

The signature from headers
