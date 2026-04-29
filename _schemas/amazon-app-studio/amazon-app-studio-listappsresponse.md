---
description: Response containing list of App Studio applications.
layout: schema
name: ListAppsResponse
properties_list:
- description: List of applications.
  name: apps
  type: array
- description: Pagination token for next page.
  name: nextToken
  type: string
provider_name: Amazon App Studio
provider_slug: amazon-app-studio
schema_file: json-schema/amazon-app-studio-listappsresponse-schema.json
slug: amazon-app-studio-listappsresponse
source_filename: amazon-app-studio-listappsresponse-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ListAppsResponse\",\n  \"description\": \"Response containing list of App Studio applications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apps\": {\n      \"type\": \"array\",\n      \"description\": \"List of applications.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/AppSummary\"\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token for next page.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-studio/refs/heads/main/json-schema/amazon-app-studio-listappsresponse-schema.json
tags:
- AWS
- Generative AI
- Internal Tools
- Low-Code
- No-Code
title: ListAppsResponse
---
