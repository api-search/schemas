---
description: Standard error response from the AppSync API
layout: schema
name: ErrorResponse
properties_list:
- description: Error message
  name: message
  type: string
- description: Error type
  name: errorType
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-error-response-schema.json
slug: appsync-error-response
source_filename: appsync-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-error-response-schema.json\",\n  \"title\": \"ErrorResponse\",\n  \"description\": \"Standard error response from the AppSync API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Error message\"\n    },\n    \"errorType\": {\n      \"type\": \"string\",\n      \"description\": \"Error type\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-error-response-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
title: ErrorResponse
---
