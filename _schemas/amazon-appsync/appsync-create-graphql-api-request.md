---
description: Request to create a GraphQL API
layout: schema
name: CreateGraphqlApiRequest
properties_list:
- description: The API name
  name: name
  type: string
- description: Default authentication type
  name: authenticationType
  type: string
- description: logConfig
  name: logConfig
  type: string
- description: Additional authentication providers
  name: additionalAuthenticationProviders
  type: array
- description: Enable X-Ray tracing
  name: xrayEnabled
  type: boolean
- description: Resource tags
  name: tags
  type: object
- description: lambdaAuthorizerConfig
  name: lambdaAuthorizerConfig
  type: string
- description: API visibility
  name: visibility
  type: string
- description: API type
  name: apiType
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-create-graphql-api-request-schema.json
slug: appsync-create-graphql-api-request
source_filename: appsync-create-graphql-api-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-create-graphql-api-request-schema.json\",\n  \"title\": \"CreateGraphqlApiRequest\",\n  \"description\": \"Request to create a GraphQL API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The API name\"\n    },\n    \"authenticationType\": {\n      \"type\": \"string\",\n      \"description\": \"Default authentication type\"\n    },\n    \"logConfig\": {\n      \"type\": \"string\",\n      \"description\": \"logConfig\"\n    },\n    \"additionalAuthenticationProviders\": {\n      \"type\": \"array\",\n      \"description\": \"Additional authentication providers\"\n    },\n    \"xrayEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable X-Ray tracing\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Resource\
  \ tags\"\n    },\n    \"lambdaAuthorizerConfig\": {\n      \"type\": \"string\",\n      \"description\": \"lambdaAuthorizerConfig\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"description\": \"API visibility\"\n    },\n    \"apiType\": {\n      \"type\": \"string\",\n      \"description\": \"API type\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-create-graphql-api-request-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: CreateGraphqlApiRequest
---
