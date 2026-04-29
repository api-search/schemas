---
description: Response with list of API keys
layout: schema
name: ListApiKeysResponse
properties_list:
- description: List of API keys
  name: apiKeys
  type: array
- description: Pagination token
  name: nextToken
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-list-api-keys-response-schema.json
slug: appsync-list-api-keys-response
source_filename: appsync-list-api-keys-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-list-api-keys-response-schema.json\",\n  \"title\": \"ListApiKeysResponse\",\n  \"description\": \"Response with list of API keys\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiKeys\": {\n      \"type\": \"array\",\n      \"description\": \"List of API keys\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-list-api-keys-response-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: ListApiKeysResponse
---
