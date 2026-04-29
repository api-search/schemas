---
description: Request to update an API key
layout: schema
name: UpdateApiKeyRequest
properties_list:
- description: Updated description
  name: description
  type: string
- description: Updated expiration timestamp
  name: expires
  type: integer
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-update-api-key-request-schema.json
slug: appsync-update-api-key-request
source_filename: appsync-update-api-key-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-update-api-key-request-schema.json\",\n  \"title\": \"UpdateApiKeyRequest\",\n  \"description\": \"Request to update an API key\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Updated description\"\n    },\n    \"expires\": {\n      \"type\": \"integer\",\n      \"description\": \"Updated expiration timestamp\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-update-api-key-request-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: UpdateApiKeyRequest
---
