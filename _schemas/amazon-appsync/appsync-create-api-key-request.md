---
description: Request to create an API key
layout: schema
name: CreateApiKeyRequest
properties_list:
- description: API key description
  name: description
  type: string
- description: Unix timestamp for expiration
  name: expires
  type: integer
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-create-api-key-request-schema.json
slug: appsync-create-api-key-request
source_filename: appsync-create-api-key-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-create-api-key-request-schema.json\",\n  \"title\": \"CreateApiKeyRequest\",\n  \"description\": \"Request to create an API key\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"API key description\"\n    },\n    \"expires\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp for expiration\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-create-api-key-request-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: CreateApiKeyRequest
---
