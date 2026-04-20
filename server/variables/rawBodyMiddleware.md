[**@bates-solutions/squareup API Reference v1.11.0**](../../README.md)

***

[@bates-solutions/squareup API Reference](../../README.md) / [server](../README.md) / rawBodyMiddleware

# Variable: rawBodyMiddleware

> `const` **rawBodyMiddleware**: `RequestHandler`

Defined in: [server/middleware/express.ts:163](https://github.com/mbates/squareup/blob/cc2848be999d186279012e73fbe300893ef84c22/src/server/middleware/express.ts#L163)

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
