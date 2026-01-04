[**@bates/squareup API Reference v0.1.0**](../../README.md)

***

[@bates/squareup API Reference](../../README.md) / [server](../README.md) / rawBodyMiddleware

# Variable: rawBodyMiddleware

> `const` **rawBodyMiddleware**: `RequestHandler`

Defined in: [src/server/middleware/express.ts:163](https://github.com/mbates/squareup/blob/982da1d528d8eb74b8387f5a958673b817575922/src/server/middleware/express.ts#L163)

Raw body parser middleware for Express

Captures the raw body before JSON parsing for signature verification.
Use this if you need to parse JSON but also need the raw body.

## Example

```typescript
import express from 'express';
import { rawBodyMiddleware } from '@bates/squareup/server';

const app = express();
app.use('/webhook', rawBodyMiddleware);
app.use('/webhook', express.json());
```
