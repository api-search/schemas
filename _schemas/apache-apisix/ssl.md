---
description: An SSL resource stores SSL certificates and keys for HTTPS traffic.
layout: schema
name: Apache APISIX SSL
properties_list:
- description: PEM-encoded SSL certificate.
  name: cert
  type: string
- description: PEM-encoded private key.
  name: key
  type: string
- description: Additional PEM-encoded certificates for multiple certificates.
  name: certs
  type: array
- description: Additional PEM-encoded private keys.
  name: keys
  type: array
- description: Server Name Indication values to match.
  name: snis
  type: array
- description: mTLS client verification configuration.
  name: client
  type: object
- description: Key-value pairs for categorization.
  name: labels
  type: object
- description: SSL status. 1 for enabled, 0 for disabled.
  name: status
  type: integer
- description: Identifies the type of certificate.
  name: type
  type: string
provider_name: Apache APISIX
provider_slug: apache-apisix
schema_file: json-schema/ssl.json
slug: ssl
tags:
- Apache
- API Gateway
- Cloud Native
- Kubernetes
- Lua
- NGINX
- Open Source
- Traffic Management
title: Apache APISIX SSL
---
