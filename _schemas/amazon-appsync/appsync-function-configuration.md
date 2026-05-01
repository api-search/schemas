---
description: A reusable pipeline function configuration
layout: schema
name: FunctionConfiguration
properties_list:
- description: The function ID
  name: functionId
  type: string
- description: The function ARN
  name: functionArn
  type: string
- description: The function name
  name: name
  type: string
- description: The function description
  name: description
  type: string
- description: The data source name
  name: dataSourceName
  type: string
- description: The request mapping template
  name: requestMappingTemplate
  type: string
- description: The response mapping template
  name: responseMappingTemplate
  type: string
- description: The function version
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
- description: The function code
  name: code
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-function-configuration-schema.json
slug: appsync-function-configuration
source_filename: appsync-function-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-function-configuration-schema.json\",\n  \"title\": \"FunctionConfiguration\",\n  \"description\": \"A reusable pipeline function configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"functionId\": {\n      \"type\": \"string\",\n      \"description\": \"The function ID\"\n    },\n    \"functionArn\": {\n      \"type\": \"string\",\n      \"description\": \"The function ARN\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The function name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The function description\"\n    },\n    \"dataSourceName\": {\n      \"type\": \"string\",\n      \"description\": \"The data source name\"\n    },\n    \"requestMappingTemplate\": {\n      \"type\": \"string\",\n      \"description\": \"The request mapping\
  \ template\"\n    },\n    \"responseMappingTemplate\": {\n      \"type\": \"string\",\n      \"description\": \"The response mapping template\"\n    },\n    \"functionVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The function version\"\n    },\n    \"syncConfig\": {\n      \"type\": \"string\",\n      \"description\": \"syncConfig\"\n    },\n    \"maxBatchSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum batch size\"\n    },\n    \"runtime\": {\n      \"type\": \"string\",\n      \"description\": \"runtime\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The function code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-function-configuration-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
title: FunctionConfiguration
---
