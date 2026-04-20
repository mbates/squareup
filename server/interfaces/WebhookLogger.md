[**@bates-solutions/squareup API Reference v1.12.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / WebhookLogger

# Interface: WebhookLogger

Defined in: [server/middleware/lambda.ts:57](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/server/middleware/lambda.ts#L57)

Logger interface for Lambda webhook handler

## Properties

### error

> **error**: (`message`, `data?`) => `void`

Defined in: [server/middleware/lambda.ts:59](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/server/middleware/lambda.ts#L59)

#### Parameters

##### message

`string`

##### data?

`Record`\<`string`, `unknown`\>

#### Returns

`void`

***

### info

> **info**: (`message`, `data?`) => `void`

Defined in: [server/middleware/lambda.ts:58](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/server/middleware/lambda.ts#L58)

#### Parameters

##### message

`string`

##### data?

`Record`\<`string`, `unknown`\>

#### Returns

`void`
