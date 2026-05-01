---
description: An API key for AppSync API authentication
layout: schema
name: ApiKey
properties_list:
- description: The API key ID
  name: id
  type: string
- description: The API key description
  name: description
  type: string
- description: Unix timestamp when the key expires
  name: expires
  type: integer
- description: Unix timestamp when the key is scheduled for deletion
  name: deletes
  type: integer
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-api-key-schema.json
slug: appsync-api-key
source_filename: appsync-api-key-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-api-key-schema.json\",\n  \"title\": \"ApiKey\",\n  \"description\": \"An API key for AppSync API authentication\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The API key ID\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The API key description\"\n    },\n    \"expires\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the key expires\"\n    },\n    \"deletes\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the key is scheduled for deletion\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-api-key-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
title: ApiKey
---
