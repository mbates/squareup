[**@bates-solutions/squareup API Reference v1.7.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / LambdaWebhookHandler

# Type Alias: LambdaWebhookHandler\<T\>

> **LambdaWebhookHandler**\<`T`\> = (`event`, `context`) => `void` \| `Promise`\<`void`\>

Defined in: [server/middleware/lambda.ts:42](https://github.com/mbates/squareup/blob/a4b8b594804c80ee4c5401fe0beb0f806e462553/src/server/middleware/lambda.ts#L42)

Handler function for Lambda webhook events

## Type Parameters

### T

`T` = `unknown`

## Parameters

### event

[`WebhookEvent`](../interfaces/WebhookEvent.md)\<`T`\>

### context

[`WebhookEventContext`](../interfaces/WebhookEventContext.md)

## Returns

`void` \| `Promise`\<`void`\>
