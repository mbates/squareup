[**@bates-solutions/squareup API Reference v1.11.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / SquareClient

# Class: SquareClient

Defined in: [core/client.ts:59](https://github.com/mbates/squareup/blob/cc2848be999d186279012e73fbe300893ef84c22/src/core/client.ts#L59)

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

Defined in: [core/client.ts:76](https://github.com/mbates/squareup/blob/cc2848be999d186279012e73fbe300893ef84c22/src/core/client.ts#L76)

#### Parameters

##### config

[`SquareClientConfig`](../interfaces/SquareClientConfig.md)

#### Returns

`SquareClient`

## Properties

### catalog

> `readonly` **catalog**: [`CatalogService`](CatalogService.md)

Defined in: [core/client.ts:69](https://github.com/mbates/squareup/blob/cc2848be999d186279012e73fbe300893ef84c22/src/core/client.ts#L69)

***

### checkout

> `readonly` **checkout**: [`CheckoutService`](CheckoutService.md)

Defined in: [core/client.ts:74](https://github.com/mbates/squareup/blob/cc2848be999d186279012e73fbe300893ef84c22/src/core/client.ts#L74)

***

### customerGroups

> `readonly` **customerGroups**: [`CustomerGroupsService`](CustomerGroupsService.md)

Defined in: [core/client.ts:68](https://github.com/mbates/squareup/blob/cc2848be999d186279012e73fbe300893ef84c22/src/core/client.ts#L68)

***

### customers

> `readonly` **customers**: [`CustomersService`](CustomersService.md)

Defined in: [core/client.ts:67](https://github.com/mbates/squareup/blob/cc2848be999d186279012e73fbe300893ef84c22/src/core/client.ts#L67)

***

### inventory

> `readonly` **inventory**: [`InventoryService`](InventoryService.md)

Defined in: [core/client.ts:70](https://github.com/mbates/squareup/blob/cc2848be999d186279012e73fbe300893ef84c22/src/core/client.ts#L70)

***

### invoices

> `readonly` **invoices**: [`InvoicesService`](InvoicesService.md)

Defined in: [core/client.ts:72](https://github.com/mbates/squareup/blob/cc2848be999d186279012e73fbe300893ef84c22/src/core/client.ts#L72)

***

### loyalty

> `readonly` **loyalty**: [`LoyaltyService`](LoyaltyService.md)

Defined in: [core/client.ts:73](https://github.com/mbates/squareup/blob/cc2848be999d186279012e73fbe300893ef84c22/src/core/client.ts#L73)

***

### orders

> `readonly` **orders**: [`OrdersService`](OrdersService.md)

Defined in: [core/client.ts:66](https://github.com/mbates/squareup/blob/cc2848be999d186279012e73fbe300893ef84c22/src/core/client.ts#L66)

***

### payments

> `readonly` **payments**: [`PaymentsService`](PaymentsService.md)

Defined in: [core/client.ts:65](https://github.com/mbates/squareup/blob/cc2848be999d186279012e73fbe300893ef84c22/src/core/client.ts#L65)

***

### subscriptions

> `readonly` **subscriptions**: [`SubscriptionsService`](SubscriptionsService.md)

Defined in: [core/client.ts:71](https://github.com/mbates/squareup/blob/cc2848be999d186279012e73fbe300893ef84c22/src/core/client.ts#L71)

## Accessors

### environment

#### Get Signature

> **get** **environment**(): [`SquareEnvironment`](../type-aliases/SquareEnvironment.md)

Defined in: [core/client.ts:123](https://github.com/mbates/squareup/blob/cc2848be999d186279012e73fbe300893ef84c22/src/core/client.ts#L123)

Get the current environment

##### Returns

[`SquareEnvironment`](../type-aliases/SquareEnvironment.md)

***

### locationId

#### Get Signature

> **get** **locationId**(): `string` \| `undefined`

Defined in: [core/client.ts:116](https://github.com/mbates/squareup/blob/cc2848be999d186279012e73fbe300893ef84c22/src/core/client.ts#L116)

Get the current location ID

##### Returns

`string` \| `undefined`

***

### sdk

#### Get Signature

> **get** **sdk**(): `SquareClient`

Defined in: [core/client.ts:109](https://github.com/mbates/squareup/blob/cc2848be999d186279012e73fbe300893ef84c22/src/core/client.ts#L109)

Get the underlying Square SDK client
Use this for advanced operations not covered by the wrapper

##### Returns

`SquareClient`
