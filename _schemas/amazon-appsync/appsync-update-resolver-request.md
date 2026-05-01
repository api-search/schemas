---
description: Request to update a resolver
layout: schema
name: UpdateResolverRequest
properties_list:
- description: Data source name
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
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-update-resolver-request-schema.json
slug: appsync-update-resolver-request
source_filename: appsync-update-resolver-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-update-resolver-request-schema.json\",\n  \"title\": \"UpdateResolverRequest\",\n  \"description\": \"Request to update a resolver\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dataSourceName\": {\n      \"type\": \"string\",\n      \"description\": \"Data source name\"\n    },\n    \"requestMappingTemplate\": {\n      \"type\": \"string\",\n      \"description\": \"Request mapping template\"\n    },\n    \"responseMappingTemplate\": {\n      \"type\": \"string\",\n      \"description\": \"Response mapping template\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Resolver kind\"\n    },\n    \"pipelineConfig\": {\n      \"type\": \"string\",\n      \"description\": \"pipelineConfig\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-update-resolver-request-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
title: UpdateResolverRequest
---
