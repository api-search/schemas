---
description: The secret management attributes.
layout: schema
name: SecretAttributes
properties_list:
- description: Determines whether the object is enabled.
  name: enabled
  type: boolean
- description: Not before date in UTC.
  name: nbf
  type: integer
- description: Expiry date in UTC.
  name: exp
  type: integer
- description: Creation time in UTC.
  name: created
  type: integer
- description: Last updated time in UTC.
  name: updated
  type: integer
- description: softDelete data retention days. Value should be >=7 and <=90 when softDelete enabled, otherwise 0.
  name: recoverableDays
  type: integer
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-secret-attributes-schema.json
slug: azure-key-vault-data-plane-secret-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecretAttributes\",\n  \"type\": \"object\",\n  \"description\": \"The secret management attributes.\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Determines whether the object is enabled.\"\n    },\n    \"nbf\": {\n      \"type\": \"integer\",\n      \"description\": \"Not before date in UTC.\"\n    },\n    \"exp\": {\n      \"type\": \"integer\",\n      \"description\": \"Expiry date in UTC.\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Creation time in UTC.\"\n    },\n    \"updated\": {\n      \"type\": \"integer\",\n      \"description\": \"Last updated time in UTC.\"\n    },\n    \"recoverableDays\": {\n      \"type\": \"integer\",\n      \"description\": \"softDelete data retention days. Value should be >=7 and <=90 when softDelete enabled, otherwise 0.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-secret-attributes-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: SecretAttributes
---
