[**@bates-solutions/squareup API Reference v1.5.1**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / SquareWebhookRequest

# Interface: SquareWebhookRequest

Defined in: [server/middleware/express.ts:13](https://github.com/mbates/squareup/blob/7abcb23f768425657eceb9d435ae63d053505602/src/server/middleware/express.ts#L13)

Extended Express Request with Square webhook data

## Extends

- `Request`

## Properties

### rawBody?

> `optional` **rawBody?**: `string`

Defined in: [server/middleware/express.ts:15](https://github.com/mbates/squareup/blob/7abcb23f768425657eceb9d435ae63d053505602/src/server/middleware/express.ts#L15)

The raw request body as a string

***

### squareEvent?

> `optional` **squareEvent?**: [`WebhookEvent`](WebhookEvent.md)\<`unknown`\>

Defined in: [server/middleware/express.ts:17](https://github.com/mbates/squareup/blob/7abcb23f768425657eceb9d435ae63d053505602/src/server/middleware/express.ts#L17)

The parsed Square webhook event
