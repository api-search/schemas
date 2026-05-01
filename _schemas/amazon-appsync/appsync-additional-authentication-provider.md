---
description: An additional authentication provider for a GraphQL API
layout: schema
name: AdditionalAuthenticationProvider
properties_list:
- description: Authentication type
  name: authenticationType
  type: string
- description: lambdaAuthorizerConfig
  name: lambdaAuthorizerConfig
  type: string
- description: userPoolConfig
  name: userPoolConfig
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-additional-authentication-provider-schema.json
slug: appsync-additional-authentication-provider
source_filename: appsync-additional-authentication-provider-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-additional-authentication-provider-schema.json\",\n  \"title\": \"AdditionalAuthenticationProvider\",\n  \"description\": \"An additional authentication provider for a GraphQL API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authenticationType\": {\n      \"type\": \"string\",\n      \"description\": \"Authentication type\"\n    },\n    \"lambdaAuthorizerConfig\": {\n      \"type\": \"string\",\n      \"description\": \"lambdaAuthorizerConfig\"\n    },\n    \"userPoolConfig\": {\n      \"type\": \"string\",\n      \"description\": \"userPoolConfig\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-additional-authentication-provider-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
title: AdditionalAuthenticationProvider
---
