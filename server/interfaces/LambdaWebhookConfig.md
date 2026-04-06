[**@bates-solutions/squareup API Reference v1.7.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / LambdaWebhookConfig

# Interface: LambdaWebhookConfig

Defined in: [server/middleware/lambda.ts:57](https://github.com/mbates/squareup/blob/a4b8b594804c80ee4c5401fe0beb0f806e462553/src/server/middleware/lambda.ts#L57)

Configuration for Lambda webhook handling

## Properties

### corsHeaders?

> `optional` **corsHeaders?**: `Record`\<`string`, `string`\>

Defined in: [server/middleware/lambda.ts:65](https://github.com/mbates/squareup/blob/a4b8b594804c80ee4c5401fe0beb0f806e462553/src/server/middleware/lambda.ts#L65)

Custom CORS headers (merged with defaults)

***

### handlers

> **handlers**: [`LambdaWebhookHandlers`](../type-aliases/LambdaWebhookHandlers.md)

Defined in: [server/middleware/lambda.ts:61](https://github.com/mbates/squareup/blob/a4b8b594804c80ee4c5401fe0beb0f806e462553/src/server/middleware/lambda.ts#L61)

Event handlers by type

***

### notificationUrl?

> `optional` **notificationUrl?**: `string`

Defined in: [server/middleware/lambda.ts:63](https://github.com/mbates/squareup/blob/a4b8b594804c80ee4c5401fe0beb0f806e462553/src/server/middleware/lambda.ts#L63)

URL where webhooks are received (for signature verification)

***

### signatureKey

> **signatureKey**: `string`

Defined in: [server/middleware/lambda.ts:59](https://github.com/mbates/squareup/blob/a4b8b594804c80ee4c5401fe0beb0f806e462553/src/server/middleware/lambda.ts#L59)

Square webhook signature key
