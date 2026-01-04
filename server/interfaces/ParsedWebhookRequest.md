[**@bates/squareup API Reference v0.1.0**](../../README.md)

***

[@bates/squareup API Reference](../../README.md) / [server](../README.md) / ParsedWebhookRequest

# Interface: ParsedWebhookRequest

Defined in: [src/server/types.ts:138](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/server/types.ts#L138)

Parsed webhook request

## Properties

### event

> **event**: [`WebhookEvent`](WebhookEvent.md)

Defined in: [src/server/types.ts:144](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/server/types.ts#L144)

Parsed event data

***

### rawBody

> **rawBody**: `string`

Defined in: [src/server/types.ts:140](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/server/types.ts#L140)

The raw request body

***

### signature

> **signature**: `string`

Defined in: [src/server/types.ts:142](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/server/types.ts#L142)

The signature from headers
