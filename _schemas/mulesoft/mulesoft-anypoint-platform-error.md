---
description: Error response from the Anypoint Platform API
layout: schema
name: Error
properties_list:
- description: HTTP status code
  name: status
  type: integer
- description: Human-readable error message
  name: message
  type: string
provider_name: MuleSoft
provider_slug: mulesoft
schema_file: json-schema/mulesoft-anypoint-platform-error-schema.json
slug: mulesoft-anypoint-platform-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"description\": \"Error response from the Anypoint Platform API\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mulesoft/refs/heads/main/json-schema/mulesoft-anypoint-platform-error-schema.json
tags:
- API Gateway
- API Management
- Enterprise
- Integration
title: Error
---
