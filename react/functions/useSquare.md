[**@bates-solutions/squareup API Reference v0.1.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [react](../README.md) / useSquare

# Function: useSquare()

> **useSquare**(): [`SquareContextValue`](../interfaces/SquareContextValue.md)

Defined in: [src/react/SquareProvider.tsx:166](https://github.com/mbates/squareup/blob/2891fe62b0e8af94ea47a5cdb6c79b3053a9ae62/src/react/SquareProvider.tsx#L166)

Hook to access Square context

## Returns

[`SquareContextValue`](../interfaces/SquareContextValue.md)

## Throws

Error if used outside of SquareProvider

## Example

```tsx
function Checkout() {
  const { sdkLoaded, payments, error } = useSquare();

  if (error) return <div>Error: {error.message}</div>;
  if (!sdkLoaded) return <div>Loading...</div>;

  return <div>Ready to accept payments!</div>;
}
```
