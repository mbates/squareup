[**@bates/squareup API Reference v0.1.0**](../../README.md)

***

[@bates/squareup API Reference](../../README.md) / [react](../README.md) / useOrders

# Function: useOrders()

> **useOrders**(`options`): [`UseOrdersReturn`](../interfaces/UseOrdersReturn.md)

Defined in: [src/react/hooks/useOrders.ts:118](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/react/hooks/useOrders.ts#L118)

Hook for managing orders via your backend API

## Parameters

### options

[`UseOrdersOptions`](../interfaces/UseOrdersOptions.md) = `{}`

Hook configuration

## Returns

[`UseOrdersReturn`](../interfaces/UseOrdersReturn.md)

Order management functions and state

## Example

```tsx
function Checkout() {
  const { cardRef, tokenize, ready } = useSquarePayment();
  const { create: createOrder, loading, error } = useOrders({
    onSuccess: (order) => console.log('Order created:', order.id),
  });

  const handleCheckout = async () => {
    const token = await tokenize();
    await createOrder({
      lineItems: [
        { name: 'Latte', amount: 450 },
        { name: 'Croissant', amount: 350 },
      ],
      paymentToken: token,
    });
  };

  return (
    <div>
      <div ref={cardRef} />
      <button onClick={handleCheckout} disabled={!ready || loading}>
        Pay $8.00
      </button>
    </div>
  );
}
```
