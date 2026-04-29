---
description: Response for retrieving an API key.
layout: schema
name: APIKeyResponse
properties_list:
- description: ''
  name: data
  type: object
- description: Array of objects related to the API key.
  name: included
  type: array
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-api-api-key-response-schema.json
slug: datadog-api-api-key-response
source_filename: datadog-api-api-key-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-api-api-key-response-schema.json\",\n  \"title\": \"APIKeyResponse\",\n  \"description\": \"Response for retrieving an API key.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"$ref\": \"#/components/schemas/FullAPIKey\"\n    },\n    \"included\": {\n      \"description\": \"Array of objects related to the API key.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/APIKeyResponseIncludedItem\"\n      },\n      \"type\": \"array\",\n      \"x-merge-override\": {\n        \"items\": false\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-api-api-key-response-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: APIKeyResponse
---
