---
description: API error response.
layout: schema
name: APIErrorResponse
properties_list:
- description: A list of errors.
  name: errors
  type: array
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-api-api-error-response-schema.json
slug: datadog-api-api-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-api-api-error-response-schema.json\",\n  \"title\": \"APIErrorResponse\",\n  \"description\": \"API error response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errors\": {\n      \"description\": \"A list of errors.\",\n      \"example\": [\n        \"Bad Request\"\n      ],\n      \"items\": {\n        \"description\": \"A list of items.\",\n        \"example\": \"Bad Request\",\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"errors\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-api-api-error-response-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: APIErrorResponse
---
