---
title: "mg_connect_http_opt()"
decl_name: "mg_connect_http_opt"
symbol_kind: "func"
signature: |
  struct mg_connection *mg_connect_http_opt(struct mg_mgr *mgr,
                                            mg_event_handler_t ev_handler,
                                            struct mg_connect_opts opts,
                                            const char *url,
                                            const char *extra_headers,
                                            const char *post_data);
---

Helper function that creates outbound HTTP connection.

Mostly identical to mg_connect_http, but allows to provide extra parameters
(for example, SSL parameters 

