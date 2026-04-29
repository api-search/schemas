---
description: Request to create a resolver
layout: schema
name: CreateResolverRequest
properties_list:
- description: The GraphQL field name
  name: fieldName
  type: string
- description: The data source name
  name: dataSourceName
  type: string
- description: Request mapping template
  name: requestMappingTemplate
  type: string
- description: Response mapping template
  name: responseMappingTemplate
  type: string
- description: Resolver kind
  name: kind
  type: string
- description: pipelineConfig
  name: pipelineConfig
  type: string
- description: syncConfig
  name: syncConfig
  type: string
- description: cachingConfig
  name: cachingConfig
  type: string
- description: Maximum batch size
  name: maxBatchSize
  type: integer
- description: runtime
  name: runtime
  type: string
- description: Function code for APPSYNC_JS runtime
  name: code
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-create-resolver-request-schema.json
slug: appsync-create-resolver-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-create-resolver-request-schema.json\",\n  \"title\": \"CreateResolverRequest\",\n  \"description\": \"Request to create a resolver\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fieldName\": {\n      \"type\": \"string\",\n      \"description\": \"The GraphQL field name\"\n    },\n    \"dataSourceName\": {\n      \"type\": \"string\",\n      \"description\": \"The data source name\"\n    },\n    \"requestMappingTemplate\": {\n      \"type\": \"string\",\n      \"description\": \"Request mapping template\"\n    },\n    \"responseMappingTemplate\": {\n      \"type\": \"string\",\n      \"description\": \"Response mapping template\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Resolver kind\"\n    },\n    \"pipelineConfig\": {\n      \"type\": \"string\",\n      \"description\": \"pipelineConfig\"\
  \n    },\n    \"syncConfig\": {\n      \"type\": \"string\",\n      \"description\": \"syncConfig\"\n    },\n    \"cachingConfig\": {\n      \"type\": \"string\",\n      \"description\": \"cachingConfig\"\n    },\n    \"maxBatchSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum batch size\"\n    },\n    \"runtime\": {\n      \"type\": \"string\",\n      \"description\": \"runtime\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Function code for APPSYNC_JS runtime\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-create-resolver-request-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: CreateResolverRequest
---
