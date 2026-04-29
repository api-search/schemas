---
description: A GraphQL API object managed by AppSync
layout: schema
name: GraphqlApi
properties_list:
- description: The API ID
  name: apiId
  type: string
- description: The API name
  name: name
  type: string
- description: The default authentication type
  name: authenticationType
  type: string
- description: The ARN of the API
  name: arn
  type: string
- description: The URIs for the API endpoint
  name: uris
  type: object
- description: Tags on the API
  name: tags
  type: object
- description: Additional authentication providers
  name: additionalAuthenticationProviders
  type: array
- description: logConfig
  name: logConfig
  type: string
- description: Whether X-Ray tracing is enabled
  name: xrayEnabled
  type: boolean
- description: WAF Web ACL ARN
  name: wafWebAclArn
  type: string
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
schema_file: json-schema/appsync-graphql-api-schema.json
slug: appsync-graphql-api
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-graphql-api-schema.json\",\n  \"title\": \"GraphqlApi\",\n  \"description\": \"A GraphQL API object managed by AppSync\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiId\": {\n      \"type\": \"string\",\n      \"description\": \"The API ID\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The API name\"\n    },\n    \"authenticationType\": {\n      \"type\": \"string\",\n      \"description\": \"The default authentication type\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the API\"\n    },\n    \"uris\": {\n      \"type\": \"object\",\n      \"description\": \"The URIs for the API endpoint\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags on the API\"\n    },\n    \"additionalAuthenticationProviders\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"Additional authentication providers\"\n    },\n    \"logConfig\": {\n      \"type\": \"string\",\n      \"description\": \"logConfig\"\n    },\n    \"xrayEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether X-Ray tracing is enabled\"\n    },\n    \"wafWebAclArn\": {\n      \"type\": \"string\",\n      \"description\": \"WAF Web ACL ARN\"\n    },\n    \"lambdaAuthorizerConfig\": {\n      \"type\": \"string\",\n      \"description\": \"lambdaAuthorizerConfig\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"description\": \"API visibility\"\n    },\n    \"apiType\": {\n      \"type\": \"string\",\n      \"description\": \"API type\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-graphql-api-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: GraphqlApi
---
