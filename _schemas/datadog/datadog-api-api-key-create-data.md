---
description: Object used to create an API key.
layout: schema
name: APIKeyCreateData
properties_list:
- description: ''
  name: attributes
  type: object
- description: ''
  name: type
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-api-api-key-create-data-schema.json
slug: datadog-api-api-key-create-data
source_filename: datadog-api-api-key-create-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-api-api-key-create-data-schema.json\",\n  \"title\": \"APIKeyCreateData\",\n  \"description\": \"Object used to create an API key.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"$ref\": \"#/components/schemas/APIKeyCreateAttributes\"\n    },\n    \"type\": {\n      \"$ref\": \"#/components/schemas/APIKeysType\"\n    }\n  },\n  \"required\": [\n    \"attributes\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-api-api-key-create-data-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: APIKeyCreateData
---
