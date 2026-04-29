---
description: Request to create a GraphQL type
layout: schema
name: CreateTypeRequest
properties_list:
- description: The type definition
  name: definition
  type: string
- description: The definition format
  name: format
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-create-type-request-schema.json
slug: appsync-create-type-request
source_filename: appsync-create-type-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-create-type-request-schema.json\",\n  \"title\": \"CreateTypeRequest\",\n  \"description\": \"Request to create a GraphQL type\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"definition\": {\n      \"type\": \"string\",\n      \"description\": \"The type definition\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"The definition format\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-create-type-request-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: CreateTypeRequest
---
