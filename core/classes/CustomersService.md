[**@bates-solutions/squareup API Reference v1.12.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / CustomersService

# Class: CustomersService

Defined in: [core/services/customers.service.ts:116](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/services/customers.service.ts#L116)

Customers service for managing Square customers

## Example

```typescript
// Create a customer
const customer = await square.customers.create({
  givenName: 'John',
  familyName: 'Doe',
  emailAddress: 'john@example.com',
});

// Search customers
const results = await square.customers.search({
  emailAddress: 'john@example.com',
});
```

## Constructors

### Constructor

> **new CustomersService**(`client`): `CustomersService`

Defined in: [core/services/customers.service.ts:117](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/services/customers.service.ts#L117)

#### Parameters

##### client

`SquareClient`

#### Returns

`CustomersService`

## Methods

### create()

> **create**(`options`): `Promise`\<`Customer`\>

Defined in: [core/services/customers.service.ts:135](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/services/customers.service.ts#L135)

Create a new customer

#### Parameters

##### options

`CreateCustomerOptions`

Customer creation options

#### Returns

`Promise`\<`Customer`\>

Created customer

#### Example

```typescript
const customer = await square.customers.create({
  givenName: 'John',
  familyName: 'Doe',
  emailAddress: 'john@example.com',
  phoneNumber: '+15551234567',
});
```

***

### delete()

> **delete**(`customerId`): `Promise`\<`void`\>

Defined in: [core/services/customers.service.ts:249](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/services/customers.service.ts#L249)

Delete a customer

#### Parameters

##### customerId

`string`

Customer ID to delete

#### Returns

`Promise`\<`void`\>

#### Example

```typescript
await square.customers.delete('CUST_123');
```

***

### get()

> **get**(`customerId`): `Promise`\<`Customer`\>

Defined in: [core/services/customers.service.ts:185](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/services/customers.service.ts#L185)

Get a customer by ID

#### Parameters

##### customerId

`string`

Customer ID

#### Returns

`Promise`\<`Customer`\>

Customer details

#### Example

```typescript
const customer = await square.customers.get('CUST_123');
```

***

### list()

> **list**(`options?`): `Promise`\<\{ `cursor?`: `string`; `customers`: `Customer`[]; \}\>

Defined in: [core/services/customers.service.ts:398](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/services/customers.service.ts#L398)

List customers with cursor-based pagination

#### Parameters

##### options?

`ListCustomersOptions`

List options including cursor for pagination

#### Returns

`Promise`\<\{ `cursor?`: `string`; `customers`: `Customer`[]; \}\>

Customers and optional cursor for next page

#### Example

```typescript
// Get first page
const page1 = await square.customers.list({ limit: 50 });

// Get next page using cursor
const page2 = await square.customers.list({ cursor: page1.cursor, limit: 50 });
```

***

### search()

> **search**(`options?`): `Promise`\<\{ `cursor?`: `string`; `data`: `Customer`[]; \}\>

Defined in: [core/services/customers.service.ts:276](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/services/customers.service.ts#L276)

Search for customers

#### Parameters

##### options?

`SearchCustomersOptions`

Search options

#### Returns

`Promise`\<\{ `cursor?`: `string`; `data`: `Customer`[]; \}\>

Matching customers with pagination

#### Example

```typescript
// Search by email
const results = await square.customers.search({
  emailAddress: 'john@example.com',
});

// Search by phone
const results = await square.customers.search({
  phoneNumber: '+15551234567',
});
```

***

### update()

> **update**(`customerId`, `options`): `Promise`\<`Customer`\>

Defined in: [core/services/customers.service.ts:213](https://github.com/mbates/squareup/blob/a23e5d04b710755974cd3f885dc527ae2c7e12be/src/core/services/customers.service.ts#L213)

Update a customer

#### Parameters

##### customerId

`string`

Customer ID to update

##### options

`UpdateCustomerOptions`

Update options

#### Returns

`Promise`\<`Customer`\>

Updated customer

#### Example

```typescript
const customer = await square.customers.update('CUST_123', {
  emailAddress: 'newemail@example.com',
});
```
