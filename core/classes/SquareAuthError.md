[**@bates/squareup API Reference v0.1.0**](../../README.md)

***

[@bates/squareup API Reference](../../README.md) / [core](../README.md) / SquareAuthError

# Class: SquareAuthError

Defined in: [src/core/errors.ts:78](https://github.com/mbates/squareup/blob/5cbceb7be75e480372e4059c7badcdbbc730e2e4/src/core/errors.ts#L78)

Authentication errors

## Extends

- [`SquareError`](SquareError.md)

## Constructors

### Constructor

> **new SquareAuthError**(`message`, `code`): `SquareAuthError`

Defined in: [src/core/errors.ts:79](https://github.com/mbates/squareup/blob/5cbceb7be75e480372e4059c7badcdbbc730e2e4/src/core/errors.ts#L79)

#### Parameters

##### message

`string`

##### code

[`SquareErrorCode`](../type-aliases/SquareErrorCode.md) = `'UNAUTHORIZED'`

#### Returns

`SquareAuthError`

#### Overrides

[`SquareError`](SquareError.md).[`constructor`](SquareError.md#constructor)

## Properties

### code

> `readonly` **code**: [`SquareErrorCode`](../type-aliases/SquareErrorCode.md)

Defined in: [src/core/errors.ts:31](https://github.com/mbates/squareup/blob/5cbceb7be75e480372e4059c7badcdbbc730e2e4/src/core/errors.ts#L31)

#### Inherited from

[`SquareError`](SquareError.md).[`code`](SquareError.md#code)

***

### details?

> `readonly` `optional` **details**: `unknown`

Defined in: [src/core/errors.ts:33](https://github.com/mbates/squareup/blob/5cbceb7be75e480372e4059c7badcdbbc730e2e4/src/core/errors.ts#L33)

#### Inherited from

[`SquareError`](SquareError.md).[`details`](SquareError.md#details)

***

### statusCode?

> `readonly` `optional` **statusCode**: `number`

Defined in: [src/core/errors.ts:32](https://github.com/mbates/squareup/blob/5cbceb7be75e480372e4059c7badcdbbc730e2e4/src/core/errors.ts#L32)

#### Inherited from

[`SquareError`](SquareError.md).[`statusCode`](SquareError.md#statuscode)
