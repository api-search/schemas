---
description: A GraphQL type definition
layout: schema
name: Type
properties_list:
- description: The type name
  name: name
  type: string
- description: Type description
  name: description
  type: string
- description: The type ARN
  name: arn
  type: string
- description: The type definition in SDL or JSON format
  name: definition
  type: string
- description: The schema format
  name: format
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-type-schema.json
slug: appsync-type
source_filename: appsync-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-type-schema.json\",\n  \"title\": \"Type\",\n  \"description\": \"A GraphQL type definition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The type name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Type description\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The type ARN\"\n    },\n    \"definition\": {\n      \"type\": \"string\",\n      \"description\": \"The type definition in SDL or JSON format\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"The schema format\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-type-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
title: Type
---
