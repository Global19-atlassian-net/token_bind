# token_binding

Provides support for the TLS Token Binding extension.

## Overview
Provides support for token binding according to the following RFCs:

- https://tools.ietf.org/html/draft-ietf-tokbind-protocol-19
- https://tools.ietf.org/html/draft-ietf-tokbind-negotiation-14
- https://tools.ietf.org/html/draft-ietf-tokbind-https-18

This token binding library links to OpenSSL/BoringSSL to provide token binding negotiation
over TLS, and provides high level functions needed to add token binding support
to HTTP applications.

This is compatible with OpenSSL versions 1.1.1 and newer.
It is implemented using the custom extension API in OpenSSL 1.1.1,
see: https://github.com/openssl/openssl/pull/3139
