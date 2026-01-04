[**@bates/squareup API Reference v0.1.0**](../../README.md)

***

[@bates/squareup API Reference](../../README.md) / [react](../README.md) / SquareProvider

# Function: SquareProvider()

> **SquareProvider**(`__namedParameters`): `Element`

Defined in: [src/react/SquareProvider.tsx:71](https://github.com/mbates/squareup/blob/5cbceb7be75e480372e4059c7badcdbbc730e2e4/src/react/SquareProvider.tsx#L71)

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
