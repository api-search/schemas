---
description: Request to update a function
layout: schema
name: UpdateFunctionRequest
properties_list:
- description: Function name
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
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-update-function-request-schema.json
slug: appsync-update-function-request
source_filename: appsync-update-function-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-update-function-request-schema.json\",\n  \"title\": \"UpdateFunctionRequest\",\n  \"description\": \"Request to update a function\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Function name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Function description\"\n    },\n    \"dataSourceName\": {\n      \"type\": \"string\",\n      \"description\": \"Data source name\"\n    },\n    \"requestMappingTemplate\": {\n      \"type\": \"string\",\n      \"description\": \"Request mapping template\"\n    },\n    \"responseMappingTemplate\": {\n      \"type\": \"string\",\n      \"description\": \"Response mapping template\"\n    },\n    \"functionVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Function\
  \ version\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-update-function-request-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
title: UpdateFunctionRequest
---
