[**@bates-solutions/squareup API Reference v0.1.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [react](../README.md) / useCustomers

# Function: useCustomers()

> **useCustomers**(`options`): [`UseCustomersReturn`](../interfaces/UseCustomersReturn.md)

Defined in: [src/react/hooks/useCustomers.ts:108](https://github.com/mbates/squareup/blob/2891fe62b0e8af94ea47a5cdb6c79b3053a9ae62/src/react/hooks/useCustomers.ts#L108)

Hook for managing customers via your backend API

## Parameters

### options

[`UseCustomersOptions`](../interfaces/UseCustomersOptions.md) = `{}`

Hook configuration

## Returns

[`UseCustomersReturn`](../interfaces/UseCustomersReturn.md)

Customer management functions and state

## Example

```tsx
function CustomerForm() {
  const { create: createCustomer, loading, error, data } = useCustomers({
    onSuccess: (customer) => console.log('Created:', customer.id),
  });

  const handleSubmit = async (formData: CustomerInput) => {
    await createCustomer({
      givenName: formData.givenName,
      familyName: formData.familyName,
      emailAddress: formData.emailAddress,
    });
  };

  return (
    <form onSubmit={handleSubmit}>
      {loading && <p>Creating customer...</p>}
      {error && <p>Error: {error.message}</p>}
      {data && <p>Customer created: {data.id}</p>}
    </form>
  );
}
```
