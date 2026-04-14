[**@bates-solutions/squareup API Reference v1.9.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / WebhookEventContext

# Interface: WebhookEventContext

Defined in: [server/middleware/lambda.ts:33](https://github.com/mbates/squareup/blob/756b613095b0aa87133212b3424e6f9269f64dfc/src/server/middleware/lambda.ts#L33)

Context passed to Lambda webhook handlers with auto-extracted entity IDs

## Properties

### customerId?

> `optional` **customerId?**: `string`

Defined in: [server/middleware/lambda.ts:36](https://github.com/mbates/squareup/blob/756b613095b0aa87133212b3424e6f9269f64dfc/src/server/middleware/lambda.ts#L36)

***

### orderId?

> `optional` **orderId?**: `string`

Defined in: [server/middleware/lambda.ts:35](https://github.com/mbates/squareup/blob/756b613095b0aa87133212b3424e6f9269f64dfc/src/server/middleware/lambda.ts#L35)

***

### paymentId?

> `optional` **paymentId?**: `string`

Defined in: [server/middleware/lambda.ts:34](https://github.com/mbates/squareup/blob/756b613095b0aa87133212b3424e6f9269f64dfc/src/server/middleware/lambda.ts#L34)
