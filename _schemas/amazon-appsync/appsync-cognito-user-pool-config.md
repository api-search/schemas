---
description: Amazon Cognito user pools configuration
layout: schema
name: CognitoUserPoolConfig
properties_list:
- description: User pool ID
  name: userPoolId
  type: string
- description: AWS Region where the user pool exists
  name: awsRegion
  type: string
- description: Regex for client IDs
  name: appIdClientRegex
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-cognito-user-pool-config-schema.json
slug: appsync-cognito-user-pool-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-cognito-user-pool-config-schema.json\",\n  \"title\": \"CognitoUserPoolConfig\",\n  \"description\": \"Amazon Cognito user pools configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userPoolId\": {\n      \"type\": \"string\",\n      \"description\": \"User pool ID\"\n    },\n    \"awsRegion\": {\n      \"type\": \"string\",\n      \"description\": \"AWS Region where the user pool exists\"\n    },\n    \"appIdClientRegex\": {\n      \"type\": \"string\",\n      \"description\": \"Regex for client IDs\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-cognito-user-pool-config-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: CognitoUserPoolConfig
---
