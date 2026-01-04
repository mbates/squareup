[**@bates/squareup API Reference v0.1.0**](../../README.md)

***

[@bates/squareup API Reference](../../README.md) / [react](../README.md) / SquareProvider

# Function: SquareProvider()

> **SquareProvider**(`__namedParameters`): `Element`

Defined in: [src/react/SquareProvider.tsx:71](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/react/SquareProvider.tsx#L71)

Square Provider component that initializes the Web Payments SDK

## Parameters

### \_\_namedParameters

[`SquareProviderProps`](../interfaces/SquareProviderProps.md)

## Returns

`Element`

## Example

```tsx
import { SquareProvider } from '@bates/squareup/react';

function App() {
  return (
    <SquareProvider
      applicationId="sq0idp-xxx"
      locationId="LXXX"
      environment="sandbox"
    >
      <Checkout />
    </SquareProvider>
  );
}
```
