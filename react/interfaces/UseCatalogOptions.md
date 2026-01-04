[**@bates-solutions/squareup API Reference v0.1.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [react](../README.md) / UseCatalogOptions

# Interface: UseCatalogOptions

Defined in: [src/react/hooks/useCatalog.ts:55](https://github.com/mbates/squareup/blob/2891fe62b0e8af94ea47a5cdb6c79b3053a9ae62/src/react/hooks/useCatalog.ts#L55)

Options for useCatalog hook

## Properties

### apiEndpoint?

> `optional` **apiEndpoint**: `string`

Defined in: [src/react/hooks/useCatalog.ts:57](https://github.com/mbates/squareup/blob/2891fe62b0e8af94ea47a5cdb6c79b3053a9ae62/src/react/hooks/useCatalog.ts#L57)

API endpoint for catalog (default: /api/catalog)

***

### fetchOnMount?

> `optional` **fetchOnMount**: `boolean`

Defined in: [src/react/hooks/useCatalog.ts:61](https://github.com/mbates/squareup/blob/2891fe62b0e8af94ea47a5cdb6c79b3053a9ae62/src/react/hooks/useCatalog.ts#L61)

Fetch on mount

***

### initialOptions?

> `optional` **initialOptions**: [`CatalogSearchOptions`](CatalogSearchOptions.md)

Defined in: [src/react/hooks/useCatalog.ts:59](https://github.com/mbates/squareup/blob/2891fe62b0e8af94ea47a5cdb6c79b3053a9ae62/src/react/hooks/useCatalog.ts#L59)

Initial search options

***

### onError()?

> `optional` **onError**: (`error`) => `void`

Defined in: [src/react/hooks/useCatalog.ts:63](https://github.com/mbates/squareup/blob/2891fe62b0e8af94ea47a5cdb6c79b3053a9ae62/src/react/hooks/useCatalog.ts#L63)

Callback on error

#### Parameters

##### error

`Error`

#### Returns

`void`
