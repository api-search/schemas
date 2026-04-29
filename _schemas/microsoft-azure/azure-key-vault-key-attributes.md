---
description: The attributes of a key.
layout: schema
name: KeyAttributes
properties_list:
- description: Whether the key is enabled.
  name: enabled
  type: boolean
- description: Not before date in UTC (Unix time).
  name: nbf
  type: integer
- description: Expiry date in UTC (Unix time).
  name: exp
  type: integer
- description: Creation time in UTC (Unix time).
  name: created
  type: integer
- description: Last updated time in UTC (Unix time).
  name: updated
  type: integer
- description: The recovery level currently in effect.
  name: recoveryLevel
  type: string
- description: The soft-delete data retention days.
  name: recoverableDays
  type: integer
- description: Whether the private key can be exported.
  name: exportable
  type: boolean
- description: The underlying HSM platform.
  name: hsmPlatform
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-key-vault-key-attributes-schema.json
slug: azure-key-vault-key-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeyAttributes\",\n  \"type\": \"object\",\n  \"description\": \"The attributes of a key.\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the key is enabled.\"\n    },\n    \"nbf\": {\n      \"type\": \"integer\",\n      \"description\": \"Not before date in UTC (Unix time).\"\n    },\n    \"exp\": {\n      \"type\": \"integer\",\n      \"description\": \"Expiry date in UTC (Unix time).\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Creation time in UTC (Unix time).\"\n    },\n    \"updated\": {\n      \"type\": \"integer\",\n      \"description\": \"Last updated time in UTC (Unix time).\"\n    },\n    \"recoveryLevel\": {\n      \"type\": \"string\",\n      \"description\": \"The recovery level currently in effect.\"\n    },\n    \"recoverableDays\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"The soft-delete data retention days.\"\n    },\n    \"exportable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the private key can be exported.\"\n    },\n    \"hsmPlatform\": {\n      \"type\": \"string\",\n      \"description\": \"The underlying HSM platform.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-key-vault-key-attributes-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: KeyAttributes
---
