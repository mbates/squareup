[**@bates-solutions/squareup API Reference v1.10.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / LambdaWebhookHandler

# Type Alias: LambdaWebhookHandler\<T\>

> **LambdaWebhookHandler**\<`T`\> = (`event`, `context`) => `void` \| `Promise`\<`void`\>

Defined in: [server/middleware/lambda.ts:42](https://github.com/mbates/squareup/blob/bd0cc77dd8a0653f0d66788f752f3f831d55e75c/src/server/middleware/lambda.ts#L42)

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
