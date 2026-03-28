[**@bates-solutions/squareup API Reference v1.3.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / WebhookVerificationResult

# Interface: WebhookVerificationResult

Defined in: [server/types.ts:128](https://github.com/mbates/squareup/blob/8b7dbd9a26fb7e3b1c18c7764f6bb54e0d3c0528/src/server/types.ts#L128)

Result of webhook verification

## Properties

### error?

> `optional` **error**: `string`

Defined in: [server/types.ts:132](https://github.com/mbates/squareup/blob/8b7dbd9a26fb7e3b1c18c7764f6bb54e0d3c0528/src/server/types.ts#L132)

Error message if invalid

***

### valid

> **valid**: `boolean`

Defined in: [server/types.ts:130](https://github.com/mbates/squareup/blob/8b7dbd9a26fb7e3b1c18c7764f6bb54e0d3c0528/src/server/types.ts#L130)

Whether the signature is valid
