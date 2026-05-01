---
description: Lambda data source configuration
layout: schema
name: LambdaDataSourceConfig
properties_list:
- description: Lambda function ARN
  name: lambdaFunctionArn
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-lambda-data-source-config-schema.json
slug: appsync-lambda-data-source-config
source_filename: appsync-lambda-data-source-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-lambda-data-source-config-schema.json\",\n  \"title\": \"LambdaDataSourceConfig\",\n  \"description\": \"Lambda data source configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lambdaFunctionArn\": {\n      \"type\": \"string\",\n      \"description\": \"Lambda function ARN\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-lambda-data-source-config-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
title: LambdaDataSourceConfig
---
