[**@bates-solutions/squareup API Reference v1.13.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / LambdaWebhookHandler

# Type Alias: LambdaWebhookHandler\<T\>

> **LambdaWebhookHandler**\<`T`\> = (`event`, `context`) => `void` \| `Promise`\<`void`\>

Defined in: [server/middleware/lambda.ts:42](https://github.com/mbates/squareup/blob/36eeb9010838e6df2f59b359e89c69f57fcea7b6/src/server/middleware/lambda.ts#L42)

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
