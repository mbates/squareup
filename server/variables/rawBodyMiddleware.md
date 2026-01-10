[**@bates-solutions/squareup API Reference v0.2.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / rawBodyMiddleware

# Variable: rawBodyMiddleware

> `const` **rawBodyMiddleware**: `RequestHandler`

Defined in: [src/server/middleware/express.ts:163](https://github.com/mbates/squareup/blob/e1717f4e682df14ec77f74c91b6d5513106fd4d4/src/server/middleware/express.ts#L163)

Raw body parser middleware for Express

Captures the raw body before JSON parsing for signature verification.
Use this if you need to parse JSON but also need the raw body.

## Example

```typescript
import express from 'express';
import { rawBodyMiddleware } from '@bates-solutions/squareup/server';

const app = express();
app.use('/webhook', rawBodyMiddleware);
app.use('/webhook', express.json());
```
