---
"cf": patch
---

Report why a request could not reach the API

A DNS failure, an untrusted TLS certificate and a refused connection were all reported as `fetch failed`. The error now includes the underlying cause, for example `fetch failed: getaddrinfo ENOTFOUND api.example.invalid`. A request that gets no response within the timeout now reports `Timeout exceeded when calling …` instead of `"timeout"`.
