[**@bates-solutions/squareup API Reference v0.2.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / WebhookVerificationResult

# Interface: WebhookVerificationResult

Defined in: [src/server/types.ts:128](https://github.com/mbates/squareup/blob/d6b2fac41166e6715afbe2a8bcbab0c784e759f8/src/server/types.ts#L128)

Result of webhook verification

## Properties

### error?

> `optional` **error**: `string`

Defined in: [src/server/types.ts:132](https://github.com/mbates/squareup/blob/d6b2fac41166e6715afbe2a8bcbab0c784e759f8/src/server/types.ts#L132)

Error message if invalid

***

### valid

> **valid**: `boolean`

Defined in: [src/server/types.ts:130](https://github.com/mbates/squareup/blob/d6b2fac41166e6715afbe2a8bcbab0c784e759f8/src/server/types.ts#L130)

Whether the signature is valid
