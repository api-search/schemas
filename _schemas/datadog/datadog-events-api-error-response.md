---
description: Standard API error response returned for failed requests
layout: schema
name: APIErrorResponse
properties_list:
- description: List of error messages describing the failure
  name: errors
  type: array
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-events-api-error-response-schema.json
slug: datadog-events-api-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-events-api-error-response-schema.json\",\n  \"title\": \"APIErrorResponse\",\n  \"description\": \"Standard API error response returned for failed requests\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"List of error messages describing the failure\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"errors\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-events-api-error-response-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: APIErrorResponse
---
