[**@bates-solutions/squareup API Reference v1.1.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / SquareWebhookRequest

# Interface: SquareWebhookRequest

Defined in: [server/middleware/express.ts:13](https://github.com/mbates/squareup/blob/dbcba9ef6bec3f860a4170a9374bb001913ef9a5/src/server/middleware/express.ts#L13)

Extended Express Request with Square webhook data

## Extends

- `Request`

## Properties

### rawBody?

> `optional` **rawBody**: `string`

Defined in: [server/middleware/express.ts:15](https://github.com/mbates/squareup/blob/dbcba9ef6bec3f860a4170a9374bb001913ef9a5/src/server/middleware/express.ts#L15)

The raw request body as a string

***

### squareEvent?

> `optional` **squareEvent**: [`WebhookEvent`](WebhookEvent.md)\<`unknown`\>

Defined in: [server/middleware/express.ts:17](https://github.com/mbates/squareup/blob/dbcba9ef6bec3f860a4170a9374bb001913ef9a5/src/server/middleware/express.ts#L17)

The parsed Square webhook event
