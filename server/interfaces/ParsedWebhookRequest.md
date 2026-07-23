[**@bates-solutions/squareup API Reference v1.14.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / ParsedWebhookRequest

# Interface: ParsedWebhookRequest

Defined in: [server/types.ts:141](https://github.com/mbates/squareup/blob/449713f7707f00c7f34a87a330a88fd0868782c8/src/server/types.ts#L141)

Parsed webhook request

## Properties

### event

> **event**: [`WebhookEvent`](WebhookEvent.md)

Defined in: [server/types.ts:147](https://github.com/mbates/squareup/blob/449713f7707f00c7f34a87a330a88fd0868782c8/src/server/types.ts#L147)

Parsed event data

***

### rawBody

> **rawBody**: `string`

Defined in: [server/types.ts:143](https://github.com/mbates/squareup/blob/449713f7707f00c7f34a87a330a88fd0868782c8/src/server/types.ts#L143)

The raw request body

***

### signature

> **signature**: `string`

Defined in: [server/types.ts:145](https://github.com/mbates/squareup/blob/449713f7707f00c7f34a87a330a88fd0868782c8/src/server/types.ts#L145)

The signature from headers
