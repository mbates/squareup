[**@bates-solutions/squareup API Reference v0.2.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / SquareClient

# Class: SquareClient

Defined in: [core/client.ts:57](https://github.com/mbates/squareup/blob/7fc1f90acc9e8ec4ffc6c0b33c0e5d3803366ae1/src/core/client.ts#L57)

Main Square client wrapper

## Example

```typescript
const square = createSquareClient({
  accessToken: process.env.SQUARE_ACCESS_TOKEN!,
  environment: 'sandbox',
  locationId: 'LXXX',
});

// Create a payment
const payment = await square.payments.create({
  sourceId: 'cnon:card-nonce-ok',
  amount: 1000, // $10.00
});
```

## Constructors

### Constructor

> **new SquareClient**(`config`): `SquareClient`

Defined in: [core/client.ts:72](https://github.com/mbates/squareup/blob/7fc1f90acc9e8ec4ffc6c0b33c0e5d3803366ae1/src/core/client.ts#L72)

#### Parameters

##### config

[`SquareClientConfig`](../interfaces/SquareClientConfig.md)

#### Returns

`SquareClient`

## Properties

### catalog

> `readonly` **catalog**: [`CatalogService`](CatalogService.md)

Defined in: [core/client.ts:66](https://github.com/mbates/squareup/blob/7fc1f90acc9e8ec4ffc6c0b33c0e5d3803366ae1/src/core/client.ts#L66)

***

### customers

> `readonly` **customers**: [`CustomersService`](CustomersService.md)

Defined in: [core/client.ts:65](https://github.com/mbates/squareup/blob/7fc1f90acc9e8ec4ffc6c0b33c0e5d3803366ae1/src/core/client.ts#L65)

***

### inventory

> `readonly` **inventory**: [`InventoryService`](InventoryService.md)

Defined in: [core/client.ts:67](https://github.com/mbates/squareup/blob/7fc1f90acc9e8ec4ffc6c0b33c0e5d3803366ae1/src/core/client.ts#L67)

***

### invoices

> `readonly` **invoices**: [`InvoicesService`](InvoicesService.md)

Defined in: [core/client.ts:69](https://github.com/mbates/squareup/blob/7fc1f90acc9e8ec4ffc6c0b33c0e5d3803366ae1/src/core/client.ts#L69)

***

### loyalty

> `readonly` **loyalty**: [`LoyaltyService`](LoyaltyService.md)

Defined in: [core/client.ts:70](https://github.com/mbates/squareup/blob/7fc1f90acc9e8ec4ffc6c0b33c0e5d3803366ae1/src/core/client.ts#L70)

***

### orders

> `readonly` **orders**: [`OrdersService`](OrdersService.md)

Defined in: [core/client.ts:64](https://github.com/mbates/squareup/blob/7fc1f90acc9e8ec4ffc6c0b33c0e5d3803366ae1/src/core/client.ts#L64)

***

### payments

> `readonly` **payments**: [`PaymentsService`](PaymentsService.md)

Defined in: [core/client.ts:63](https://github.com/mbates/squareup/blob/7fc1f90acc9e8ec4ffc6c0b33c0e5d3803366ae1/src/core/client.ts#L63)

***

### subscriptions

> `readonly` **subscriptions**: [`SubscriptionsService`](SubscriptionsService.md)

Defined in: [core/client.ts:68](https://github.com/mbates/squareup/blob/7fc1f90acc9e8ec4ffc6c0b33c0e5d3803366ae1/src/core/client.ts#L68)

## Accessors

### environment

#### Get Signature

> **get** **environment**(): [`SquareEnvironment`](../type-aliases/SquareEnvironment.md)

Defined in: [core/client.ts:117](https://github.com/mbates/squareup/blob/7fc1f90acc9e8ec4ffc6c0b33c0e5d3803366ae1/src/core/client.ts#L117)

Get the current environment

##### Returns

[`SquareEnvironment`](../type-aliases/SquareEnvironment.md)

***

### locationId

#### Get Signature

> **get** **locationId**(): `string` \| `undefined`

Defined in: [core/client.ts:110](https://github.com/mbates/squareup/blob/7fc1f90acc9e8ec4ffc6c0b33c0e5d3803366ae1/src/core/client.ts#L110)

Get the current location ID

##### Returns

`string` \| `undefined`

***

### sdk

#### Get Signature

> **get** **sdk**(): `SquareClient`

Defined in: [core/client.ts:103](https://github.com/mbates/squareup/blob/7fc1f90acc9e8ec4ffc6c0b33c0e5d3803366ae1/src/core/client.ts#L103)

Get the underlying Square SDK client
Use this for advanced operations not covered by the wrapper

##### Returns

`SquareClient`
