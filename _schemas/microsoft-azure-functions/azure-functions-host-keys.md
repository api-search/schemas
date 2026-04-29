---
description: Functions host level keys.
layout: schema
name: HostKeys
properties_list:
- description: Secret key.
  name: masterKey
  type: string
- description: Host level function keys.
  name: functionKeys
  type: object
- description: System keys.
  name: systemKeys
  type: object
provider_name: Microsoft Azure Functions
provider_slug: microsoft-azure-functions
schema_file: json-schema/azure-functions-host-keys-schema.json
slug: azure-functions-host-keys
source_filename: azure-functions-host-keys-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-host-keys-schema.json\",\n  \"title\": \"HostKeys\",\n  \"description\": \"Functions host level keys.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"masterKey\": {\n      \"type\": \"string\",\n      \"description\": \"Secret key.\"\n    },\n    \"functionKeys\": {\n      \"type\": \"object\",\n      \"description\": \"Host level function keys.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"systemKeys\": {\n      \"type\": \"object\",\n      \"description\": \"System keys.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-host-keys-schema.json
tags:
- Azure
- Cloud
- Compute
- Event-Driven
- Microsoft
- Serverless
title: HostKeys
---
