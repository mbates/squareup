[**@bates-solutions/squareup API Reference v0.2.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / SquareWebhookRequest

# Interface: SquareWebhookRequest

Defined in: [src/server/middleware/express.ts:13](https://github.com/mbates/squareup/blob/e1717f4e682df14ec77f74c91b6d5513106fd4d4/src/server/middleware/express.ts#L13)

Extended Express Request with Square webhook data

## Extends

- `Request`

## Properties

### rawBody?

> `optional` **rawBody**: `string`

Defined in: [src/server/middleware/express.ts:15](https://github.com/mbates/squareup/blob/e1717f4e682df14ec77f74c91b6d5513106fd4d4/src/server/middleware/express.ts#L15)

The raw request body as a string

***

### squareEvent?

> `optional` **squareEvent**: [`WebhookEvent`](WebhookEvent.md)\<`unknown`\>

Defined in: [src/server/middleware/express.ts:17](https://github.com/mbates/squareup/blob/e1717f4e682df14ec77f74c91b6d5513106fd4d4/src/server/middleware/express.ts#L17)

The parsed Square webhook event
