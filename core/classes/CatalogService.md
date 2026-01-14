[**@bates-solutions/squareup API Reference v1.0.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [core](../README.md) / CatalogService

# Class: CatalogService

Defined in: [core/services/catalog.service.ts:152](https://github.com/mbates/squareup/blob/32b2a6cc46d36384f60a869a504a33fd25157827/src/core/services/catalog.service.ts#L152)

Catalog service for managing Square catalog items

## Example

```typescript
// Create an item with variations
const item = await square.catalog.createItem({
  name: 'Coffee',
  variations: [
    { name: 'Small', price: 350 },
    { name: 'Large', price: 450 },
  ],
});

// Search items
const results = await square.catalog.search({
  objectTypes: ['ITEM'],
  query: 'coffee',
});
```

## Constructors

### Constructor

> **new CatalogService**(`client`): `CatalogService`

Defined in: [core/services/catalog.service.ts:153](https://github.com/mbates/squareup/blob/32b2a6cc46d36384f60a869a504a33fd25157827/src/core/services/catalog.service.ts#L153)

#### Parameters

##### client

`SquareClient`

#### Returns

`CatalogService`

## Methods

### batchGet()

> **batchGet**(`objectIds`): `Promise`\<`CatalogObject`[]\>

Defined in: [core/services/catalog.service.ts:454](https://github.com/mbates/squareup/blob/32b2a6cc46d36384f60a869a504a33fd25157827/src/core/services/catalog.service.ts#L454)

Batch retrieve multiple catalog objects

#### Parameters

##### objectIds

`string`[]

Array of object IDs to retrieve

#### Returns

`Promise`\<`CatalogObject`[]\>

Array of catalog objects

#### Example

```typescript
const items = await square.catalog.batchGet(['ITEM_1', 'ITEM_2', 'ITEM_3']);
```

***

### createCategory()

> **createCategory**(`options`): `Promise`\<`CatalogObject`\>

Defined in: [core/services/catalog.service.ts:235](https://github.com/mbates/squareup/blob/32b2a6cc46d36384f60a869a504a33fd25157827/src/core/services/catalog.service.ts#L235)

Create a category

#### Parameters

##### options

`CreateCategoryOptions`

Category creation options

#### Returns

`Promise`\<`CatalogObject`\>

Created category

#### Example

```typescript
const category = await square.catalog.createCategory({
  name: 'Beverages',
});
```

***

### createItem()

> **createItem**(`options`): `Promise`\<`CatalogObject`\>

Defined in: [core/services/catalog.service.ts:174](https://github.com/mbates/squareup/blob/32b2a6cc46d36384f60a869a504a33fd25157827/src/core/services/catalog.service.ts#L174)

Create a catalog item with variations

#### Parameters

##### options

`CreateCatalogItemOptions`

Item creation options

#### Returns

`Promise`\<`CatalogObject`\>

Created catalog object

#### Example

```typescript
const item = await square.catalog.createItem({
  name: 'Latte',
  description: 'Espresso with steamed milk',
  variations: [
    { name: 'Small', price: 400, sku: 'LATTE-S' },
    { name: 'Medium', price: 500, sku: 'LATTE-M' },
    { name: 'Large', price: 600, sku: 'LATTE-L' },
  ],
});
```

***

### delete()

> **delete**(`objectId`): `Promise`\<`void`\>

Defined in: [core/services/catalog.service.ts:352](https://github.com/mbates/squareup/blob/32b2a6cc46d36384f60a869a504a33fd25157827/src/core/services/catalog.service.ts#L352)

Delete a catalog object

#### Parameters

##### objectId

`string`

Catalog object ID to delete

#### Returns

`Promise`\<`void`\>

#### Example

```typescript
await square.catalog.delete('ITEM_123');
```

***

### get()

> **get**(`objectId`): `Promise`\<`CatalogObject`\>

Defined in: [core/services/catalog.service.ts:325](https://github.com/mbates/squareup/blob/32b2a6cc46d36384f60a869a504a33fd25157827/src/core/services/catalog.service.ts#L325)

Get a catalog object by ID

#### Parameters

##### objectId

`string`

Catalog object ID

#### Returns

`Promise`\<`CatalogObject`\>

Catalog object

#### Example

```typescript
const item = await square.catalog.get('ITEM_123');
```

***

### list()

> **list**(`objectType`, `options?`): `Promise`\<`CatalogObject`[]\>

Defined in: [core/services/catalog.service.ts:418](https://github.com/mbates/squareup/blob/32b2a6cc46d36384f60a869a504a33fd25157827/src/core/services/catalog.service.ts#L418)

List all catalog objects of a specific type

#### Parameters

##### objectType

`CatalogObjectType`

Type of objects to list

##### options?

List options

###### limit?

`number`

#### Returns

`Promise`\<`CatalogObject`[]\>

Array of catalog objects

#### Example

```typescript
const items = await square.catalog.list('ITEM', { limit: 50 });
```

***

### search()

> **search**(`options?`): `Promise`\<\{ `cursor?`: `string`; `data`: `CatalogObject`[]; \}\>

Defined in: [core/services/catalog.service.ts:380](https://github.com/mbates/squareup/blob/32b2a6cc46d36384f60a869a504a33fd25157827/src/core/services/catalog.service.ts#L380)

Search the catalog

#### Parameters

##### options?

`SearchCatalogOptions`

Search options

#### Returns

`Promise`\<\{ `cursor?`: `string`; `data`: `CatalogObject`[]; \}\>

Matching catalog objects with pagination

#### Example

```typescript
// Search for items
const results = await square.catalog.search({
  objectTypes: ['ITEM'],
  query: 'coffee',
});

// Get all categories
const categories = await square.catalog.search({
  objectTypes: ['CATEGORY'],
});
```

***

### upsert()

> **upsert**(`catalogObject`, `idempotencyKey?`): `Promise`\<`CatalogObject`\>

Defined in: [core/services/catalog.service.ts:294](https://github.com/mbates/squareup/blob/32b2a6cc46d36384f60a869a504a33fd25157827/src/core/services/catalog.service.ts#L294)

Upsert (create or update) a catalog object

#### Parameters

##### catalogObject

`CatalogObject`

The catalog object to upsert

##### idempotencyKey?

`string`

Optional idempotency key

#### Returns

`Promise`\<`CatalogObject`\>

The upserted catalog object

#### Example

```typescript
// Update an existing item's custom attributes
const updatedItem = await square.catalog.upsert({
  type: 'ITEM',
  id: 'EXISTING_ITEM_ID',
  version: existingItem.version,
  customAttributeValues: {
    'Square:some-key': { stringValue: 'new value' }
  },
  itemData: existingItem.itemData,
});

// Update a variation price
const updatedVariation = await square.catalog.upsert({
  type: 'ITEM_VARIATION',
  id: 'EXISTING_VARIATION_ID',
  version: existingVariation.version,
  itemVariationData: {
    ...existingVariation.itemVariationData,
    priceMoney: { amount: BigInt(500), currency: 'USD' },
  },
});
```
