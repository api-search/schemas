---
description: Error response from the Looker API
layout: schema
name: ErrorResponse
properties_list:
- description: Human-readable error message
  name: message
  type: string
- description: URL to relevant API documentation
  name: documentation_url
  type: string
provider_name: Looker
provider_slug: looker
schema_file: json-schema/looker-error-response-schema.json
slug: looker-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Error response from the Looker API\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\"\n    },\n    \"documentation_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to relevant API documentation\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/json-schema/looker-error-response-schema.json
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
title: ErrorResponse
---
