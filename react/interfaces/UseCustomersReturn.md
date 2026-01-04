[**@bates-solutions/squareup API Reference v0.1.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [react](../README.md) / UseCustomersReturn

# Interface: UseCustomersReturn

Defined in: [src/react/hooks/useCustomers.ts:64](https://github.com/mbates/squareup/blob/51442cfe91df1809d815d2acb88b04112b6ed3da/src/react/hooks/useCustomers.ts#L64)

Return type for useCustomers hook

## Extends

- [`MutationState`](MutationState.md)\<[`CustomerResponse`](CustomerResponse.md)\>

## Properties

### create()

> **create**: (`input`) => `Promise`\<[`CustomerResponse`](CustomerResponse.md)\>

Defined in: [src/react/hooks/useCustomers.ts:66](https://github.com/mbates/squareup/blob/51442cfe91df1809d815d2acb88b04112b6ed3da/src/react/hooks/useCustomers.ts#L66)

Create a new customer

#### Parameters

##### input

[`CustomerInput`](CustomerInput.md)

#### Returns

`Promise`\<[`CustomerResponse`](CustomerResponse.md)\>

***

### data

> **data**: [`CustomerResponse`](CustomerResponse.md) \| `null`

Defined in: [src/react/types.ts:208](https://github.com/mbates/squareup/blob/51442cfe91df1809d815d2acb88b04112b6ed3da/src/react/types.ts#L208)

#### Inherited from

[`MutationState`](MutationState.md).[`data`](MutationState.md#data)

***

### error

> **error**: `Error` \| `null`

Defined in: [src/react/types.ts:209](https://github.com/mbates/squareup/blob/51442cfe91df1809d815d2acb88b04112b6ed3da/src/react/types.ts#L209)

#### Inherited from

[`MutationState`](MutationState.md).[`error`](MutationState.md#error)

***

### get()

> **get**: (`customerId`) => `Promise`\<[`CustomerResponse`](CustomerResponse.md)\>

Defined in: [src/react/hooks/useCustomers.ts:68](https://github.com/mbates/squareup/blob/51442cfe91df1809d815d2acb88b04112b6ed3da/src/react/hooks/useCustomers.ts#L68)

Get a customer by ID

#### Parameters

##### customerId

`string`

#### Returns

`Promise`\<[`CustomerResponse`](CustomerResponse.md)\>

***

### loading

> **loading**: `boolean`

Defined in: [src/react/types.ts:210](https://github.com/mbates/squareup/blob/51442cfe91df1809d815d2acb88b04112b6ed3da/src/react/types.ts#L210)

#### Inherited from

[`MutationState`](MutationState.md).[`loading`](MutationState.md#loading)

***

### reset()

> **reset**: () => `void`

Defined in: [src/react/hooks/useCustomers.ts:74](https://github.com/mbates/squareup/blob/51442cfe91df1809d815d2acb88b04112b6ed3da/src/react/hooks/useCustomers.ts#L74)

Reset the hook state

#### Returns

`void`

***

### search()

> **search**: (`query`) => `Promise`\<[`CustomerResponse`](CustomerResponse.md)[]\>

Defined in: [src/react/hooks/useCustomers.ts:72](https://github.com/mbates/squareup/blob/51442cfe91df1809d815d2acb88b04112b6ed3da/src/react/hooks/useCustomers.ts#L72)

Search for customers

#### Parameters

##### query

###### email?

`string`

###### phone?

`string`

#### Returns

`Promise`\<[`CustomerResponse`](CustomerResponse.md)[]\>

***

### update()

> **update**: (`customerId`, `input`) => `Promise`\<[`CustomerResponse`](CustomerResponse.md)\>

Defined in: [src/react/hooks/useCustomers.ts:70](https://github.com/mbates/squareup/blob/51442cfe91df1809d815d2acb88b04112b6ed3da/src/react/hooks/useCustomers.ts#L70)

Update a customer

#### Parameters

##### customerId

`string`

##### input

[`CustomerInput`](CustomerInput.md)

#### Returns

`Promise`\<[`CustomerResponse`](CustomerResponse.md)\>
