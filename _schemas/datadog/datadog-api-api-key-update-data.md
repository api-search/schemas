---
description: Object used to update an API key.
layout: schema
name: APIKeyUpdateData
properties_list:
- description: ''
  name: attributes
  type: object
- description: ID of the API key.
  name: id
  type: string
- description: ''
  name: type
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-api-api-key-update-data-schema.json
slug: datadog-api-api-key-update-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-api-api-key-update-data-schema.json\",\n  \"title\": \"APIKeyUpdateData\",\n  \"description\": \"Object used to update an API key.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"$ref\": \"#/components/schemas/APIKeyUpdateAttributes\"\n    },\n    \"id\": {\n      \"description\": \"ID of the API key.\",\n      \"example\": \"00112233-4455-6677-8899-aabbccddeeff\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"$ref\": \"#/components/schemas/APIKeysType\"\n    }\n  },\n  \"required\": [\n    \"attributes\",\n    \"id\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-api-api-key-update-data-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: APIKeyUpdateData
---
