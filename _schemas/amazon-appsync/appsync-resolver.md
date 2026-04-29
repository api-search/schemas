---
description: A resolver for a GraphQL field
layout: schema
name: Resolver
properties_list:
- description: The GraphQL type name
  name: typeName
  type: string
- description: The GraphQL field name
  name: fieldName
  type: string
- description: The data source name
  name: dataSourceName
  type: string
- description: The resolver ARN
  name: resolverArn
  type: string
- description: The request mapping template
  name: requestMappingTemplate
  type: string
- description: The response mapping template
  name: responseMappingTemplate
  type: string
- description: The resolver kind
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
- description: The function code
  name: code
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-resolver-schema.json
slug: appsync-resolver
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-resolver-schema.json\",\n  \"title\": \"Resolver\",\n  \"description\": \"A resolver for a GraphQL field\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"typeName\": {\n      \"type\": \"string\",\n      \"description\": \"The GraphQL type name\"\n    },\n    \"fieldName\": {\n      \"type\": \"string\",\n      \"description\": \"The GraphQL field name\"\n    },\n    \"dataSourceName\": {\n      \"type\": \"string\",\n      \"description\": \"The data source name\"\n    },\n    \"resolverArn\": {\n      \"type\": \"string\",\n      \"description\": \"The resolver ARN\"\n    },\n    \"requestMappingTemplate\": {\n      \"type\": \"string\",\n      \"description\": \"The request mapping template\"\n    },\n    \"responseMappingTemplate\": {\n      \"type\": \"string\",\n      \"description\": \"The response mapping template\"\
  \n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The resolver kind\"\n    },\n    \"pipelineConfig\": {\n      \"type\": \"string\",\n      \"description\": \"pipelineConfig\"\n    },\n    \"syncConfig\": {\n      \"type\": \"string\",\n      \"description\": \"syncConfig\"\n    },\n    \"cachingConfig\": {\n      \"type\": \"string\",\n      \"description\": \"cachingConfig\"\n    },\n    \"maxBatchSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum batch size\"\n    },\n    \"runtime\": {\n      \"type\": \"string\",\n      \"description\": \"runtime\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The function code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-resolver-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: Resolver
---
