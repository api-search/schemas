---
description: Request to create a pipeline function
layout: schema
name: CreateFunctionRequest
properties_list:
- description: The function name
  name: name
  type: string
- description: Function description
  name: description
  type: string
- description: Data source name
  name: dataSourceName
  type: string
- description: Request mapping template
  name: requestMappingTemplate
  type: string
- description: Response mapping template
  name: responseMappingTemplate
  type: string
- description: Function version
  name: functionVersion
  type: string
- description: syncConfig
  name: syncConfig
  type: string
- description: Maximum batch size
  name: maxBatchSize
  type: integer
- description: runtime
  name: runtime
  type: string
- description: Function code
  name: code
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-create-function-request-schema.json
slug: appsync-create-function-request
source_filename: appsync-create-function-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-create-function-request-schema.json\",\n  \"title\": \"CreateFunctionRequest\",\n  \"description\": \"Request to create a pipeline function\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The function name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Function description\"\n    },\n    \"dataSourceName\": {\n      \"type\": \"string\",\n      \"description\": \"Data source name\"\n    },\n    \"requestMappingTemplate\": {\n      \"type\": \"string\",\n      \"description\": \"Request mapping template\"\n    },\n    \"responseMappingTemplate\": {\n      \"type\": \"string\",\n      \"description\": \"Response mapping template\"\n    },\n    \"functionVersion\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Function version\"\n    },\n    \"syncConfig\": {\n      \"type\": \"string\",\n      \"description\": \"syncConfig\"\n    },\n    \"maxBatchSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum batch size\"\n    },\n    \"runtime\": {\n      \"type\": \"string\",\n      \"description\": \"runtime\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Function code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-create-function-request-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
title: CreateFunctionRequest
---
