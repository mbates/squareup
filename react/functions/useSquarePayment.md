[**@bates-solutions/squareup API Reference v0.1.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [react](../README.md) / useSquarePayment

# Function: useSquarePayment()

> **useSquarePayment**(`options`): [`UseSquarePaymentReturn`](../interfaces/UseSquarePaymentReturn.md)

Defined in: [src/react/hooks/useSquarePayment.ts:55](https://github.com/mbates/squareup/blob/2891fe62b0e8af94ea47a5cdb6c79b3053a9ae62/src/react/hooks/useSquarePayment.ts#L55)

Hook for integrating Square Web Payments SDK card input

## Parameters

### options

[`UseSquarePaymentOptions`](../interfaces/UseSquarePaymentOptions.md) = `{}`

Configuration options

## Returns

[`UseSquarePaymentReturn`](../interfaces/UseSquarePaymentReturn.md)

Card input ref, tokenize function, and state

## Example

```tsx
function Checkout() {
  const { cardRef, tokenize, ready, loading, error } = useSquarePayment({
    onReady: () => console.log('Card input ready'),
    onTokenize: (token) => console.log('Token:', token),
    onError: (err) => console.error('Error:', err),
  });

  const handlePay = async () => {
    try {
      const token = await tokenize();
      // Send token to your server to complete payment
    } catch (err) {
      console.error('Tokenization failed:', err);
    }
  };

  return (
    <div>
      <div ref={cardRef} />
      <button onClick={handlePay} disabled={!ready || loading}>
        Pay
      </button>
      {error && <p>Error: {error.message}</p>}
    </div>
  );
}
```
