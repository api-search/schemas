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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/apache-apisix/blob/main/json-schema/ssl.json\",\n  \"title\": \"Apache APISIX SSL\",\n  \"description\": \"An SSL resource stores SSL certificates and keys for HTTPS traffic.\",\n  \"type\": \"object\",\n  \"required\": [\"cert\", \"key\", \"snis\"],\n  \"properties\": {\n    \"cert\": {\n      \"type\": \"string\",\n      \"description\": \"PEM-encoded SSL certificate.\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"PEM-encoded private key.\"\n    },\n    \"certs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Additional PEM-encoded certificates for multiple certificates.\"\n    },\n    \"keys\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Additional PEM-encoded private keys.\"\n    },\n\
  \    \"snis\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Server Name Indication values to match.\"\n    },\n    \"client\": {\n      \"type\": \"object\",\n      \"description\": \"mTLS client verification configuration.\",\n      \"properties\": {\n        \"ca\": {\n          \"type\": \"string\",\n          \"description\": \"PEM-encoded CA certificate for client verification.\"\n        },\n        \"depth\": {\n          \"type\": \"integer\",\n          \"default\": 1,\n          \"description\": \"Maximum length of the client certificate chain.\"\n        }\n      }\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key-value pairs for categorization.\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"enum\": [0, 1],\n      \"default\": 1,\n      \"description\": \"SSL status. 1 for enabled,\
  \ 0 for disabled.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"server\", \"client\"],\n      \"default\": \"server\",\n      \"description\": \"Identifies the type of certificate.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/json-schema/ssl.json
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
