---
title: "mg_next()"
decl_name: "mg_next"
symbol_kind: "func"
signature: |
  struct mg_connection *mg_next(struct mg_mgr *, struct mg_connection *);
---

Iterate over all active connections.

Returns next connection from the list
of active connections, or `NULL` if there is no more connections. Below
is the iteration idiom:

```c
for (c = mg_next(srv, NULL); c != NULL; c = mg_next(srv, c)) {
  // Do something with connection `c`
}
``` 

