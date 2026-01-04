[**@bates/squareup API Reference v0.1.0**](../../README.md)

***

[@bates/squareup API Reference](../../README.md) / [angular](../README.md) / Payments

# Interface: Payments

Defined in: [src/angular/types.ts:24](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/angular/types.ts#L24)

Square Web Payments SDK types

## Methods

### applePay()

> **applePay**(`options`): `Promise`\<[`ApplePay`](ApplePay.md)\>

Defined in: [src/angular/types.ts:27](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/angular/types.ts#L27)

#### Parameters

##### options

[`ApplePayOptions`](ApplePayOptions.md)

#### Returns

`Promise`\<[`ApplePay`](ApplePay.md)\>

***

### card()

> **card**(`options?`): `Promise`\<[`Card`](Card.md)\>

Defined in: [src/angular/types.ts:25](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/angular/types.ts#L25)

#### Parameters

##### options?

[`CardOptions`](CardOptions.md)

#### Returns

`Promise`\<[`Card`](Card.md)\>

***

### googlePay()

> **googlePay**(`options`): `Promise`\<[`GooglePay`](GooglePay.md)\>

Defined in: [src/angular/types.ts:26](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/angular/types.ts#L26)

#### Parameters

##### options

[`GooglePayOptions`](GooglePayOptions.md)

#### Returns

`Promise`\<[`GooglePay`](GooglePay.md)\>
