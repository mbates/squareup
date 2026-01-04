[**@bates/squareup API Reference v0.1.0**](../../README.md)

***

[@bates/squareup API Reference](../../README.md) / [react](../README.md) / CardInput

# Variable: CardInput

> `const` **CardInput**: `ForwardRefExoticComponent`\<[`CardInputProps`](../interfaces/CardInputProps.md) & `RefAttributes`\<[`CardInputHandle`](../interfaces/CardInputHandle.md)\>\>

Defined in: [src/react/components/CardInput.tsx:72](https://github.com/mbates/squareup/blob/5cbceb7be75e480372e4059c7badcdbbc730e2e4/src/react/components/CardInput.tsx#L72)

Pre-built card input component using Square Web Payments SDK

## Example

```tsx
import { CardInput, CardInputHandle } from '@bates/squareup/react';

function Checkout() {
  const cardRef = useRef<CardInputHandle>(null);

  const handlePay = async () => {
    if (!cardRef.current?.ready) return;

    try {
      const token = await cardRef.current.tokenize();
      // Send token to your server
      console.log('Token:', token);
    } catch (err) {
      console.error('Tokenization failed:', err);
    }
  };

  return (
    <div>
      <CardInput
        ref={cardRef}
        onReady={() => console.log('Card input ready')}
        onError={(err) => console.error('Error:', err)}
      />
      <button onClick={handlePay}>Pay</button>
    </div>
  );
}
```
