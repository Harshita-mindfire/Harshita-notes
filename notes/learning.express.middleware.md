---
id: 5jsgly6zxbtm0cgw8ljs0re
title: Middleware
desc: ''
updated: 1671459779593
created: 1671459779593
---
- middleware is a func that can intercept the request response cycle.
- has access to req and response objects
- take 3 params, req, res, next

## Existing examples
- morgan: third party dev logging middleware
- `app.use(express.json())`: in order to use req.body you need express's built-in body parser middleware. If we don't use this, fetching `req.body` for a route gives undefined.



