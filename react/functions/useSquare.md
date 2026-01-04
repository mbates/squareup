[**@bates/squareup API Reference v0.1.0**](../../README.md)

***

[@bates/squareup API Reference](../../README.md) / [react](../README.md) / useSquare

# Function: useSquare()

> **useSquare**(): [`SquareContextValue`](../interfaces/SquareContextValue.md)

Defined in: [src/react/SquareProvider.tsx:166](https://github.com/mbates/squareup/blob/5cbceb7be75e480372e4059c7badcdbbc730e2e4/src/react/SquareProvider.tsx#L166)

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
