---
description: Request used to create an API key.
layout: schema
name: APIKeyCreateRequest
properties_list:
- description: ''
  name: data
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-api-api-key-create-request-schema.json
slug: datadog-api-api-key-create-request
source_filename: datadog-api-api-key-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-api-api-key-create-request-schema.json\",\n  \"title\": \"APIKeyCreateRequest\",\n  \"description\": \"Request used to create an API key.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"$ref\": \"#/components/schemas/APIKeyCreateData\"\n    }\n  },\n  \"required\": [\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-api-api-key-create-request-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: APIKeyCreateRequest
---
