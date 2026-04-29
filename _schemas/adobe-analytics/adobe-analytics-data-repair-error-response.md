---
description: Error response from the API
layout: schema
name: ErrorResponse
properties_list:
- description: Machine-readable error code
  name: errorCode
  type: string
- description: Human-readable error message
  name: errorDescription
  type: string
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-data-repair-error-response-schema.json
slug: adobe-analytics-data-repair-error-response
source_filename: adobe-analytics-data-repair-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Error response from the API\",\n  \"properties\": {\n    \"errorCode\": {\n      \"type\": \"string\",\n      \"description\": \"Machine-readable error code\",\n      \"example\": \"example_value\"\n    },\n    \"errorDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-data-repair-error-response-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: ErrorResponse
---
