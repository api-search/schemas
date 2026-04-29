---
description: ''
layout: schema
name: SecretAttributes
properties_list:
- description: The name of the secret.
  name: name
  type: string
- description: The type of secret.
  name: type_of
  type: string
- description: The exchange status of the secret.
  name: status
  type: string
- description: The credential payload, varies by secret type.
  name: credentials
  type: object
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/reactor-secret-attributes-schema.json
slug: reactor-secret-attributes
source_filename: reactor-secret-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecretAttributes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the secret.\"\n    },\n    \"type_of\": {\n      \"type\": \"string\",\n      \"description\": \"The type of secret.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The exchange status of the secret.\"\n    },\n    \"credentials\": {\n      \"type\": \"object\",\n      \"description\": \"The credential payload, varies by secret type.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/reactor-secret-attributes-schema.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: SecretAttributes
---
