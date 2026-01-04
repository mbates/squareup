[**@bates-solutions/squareup API Reference v0.1.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [react](../README.md) / PaymentButton

# Function: PaymentButton()

> **PaymentButton**(`__namedParameters`): `Element`

Defined in: [src/react/components/PaymentButton.tsx:74](https://github.com/mbates/squareup/blob/2891fe62b0e8af94ea47a5cdb6c79b3053a9ae62/src/react/components/PaymentButton.tsx#L74)

Digital wallet payment button (Google Pay / Apple Pay)

## Parameters

### \_\_namedParameters

[`PaymentButtonProps`](../interfaces/PaymentButtonProps.md)

## Returns

`Element`

## Example

```tsx
import { PaymentButton } from '@bates-solutions/squareup/react';

function Checkout() {
  const handlePayment = async (token: string) => {
    // Send token to your server to complete payment
    const response = await fetch('/api/payments', {
      method: 'POST',
      headers: { 'Content-Type': 'application/json' },
      body: JSON.stringify({ sourceId: token, amount: 1000 }),
    });
  };

  return (
    <div>
      <PaymentButton
        type="googlePay"
        amount={1000}
        currency="USD"
        onPayment={handlePayment}
        onError={(err) => console.error('Error:', err)}
      />
      <PaymentButton
        type="applePay"
        amount={1000}
        currency="USD"
        onPayment={handlePayment}
        onError={(err) => console.error('Error:', err)}
      />
    </div>
  );
}
```
