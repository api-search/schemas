---
description: Request to create a data source
layout: schema
name: CreateDataSourceRequest
properties_list:
- description: The data source name
  name: name
  type: string
- description: The data source description
  name: description
  type: string
- description: The data source type
  name: type
  type: string
- description: IAM role ARN for AppSync to assume
  name: serviceRoleArn
  type: string
- description: dynamodbConfig
  name: dynamodbConfig
  type: string
- description: lambdaConfig
  name: lambdaConfig
  type: string
- description: httpConfig
  name: httpConfig
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-create-data-source-request-schema.json
slug: appsync-create-data-source-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-create-data-source-request-schema.json\",\n  \"title\": \"CreateDataSourceRequest\",\n  \"description\": \"Request to create a data source\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The data source name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The data source description\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The data source type\"\n    },\n    \"serviceRoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"IAM role ARN for AppSync to assume\"\n    },\n    \"dynamodbConfig\": {\n      \"type\": \"string\",\n      \"description\": \"dynamodbConfig\"\n    },\n    \"lambdaConfig\": {\n      \"type\": \"string\",\n      \"description\": \"lambdaConfig\"\
  \n    },\n    \"httpConfig\": {\n      \"type\": \"string\",\n      \"description\": \"httpConfig\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-create-data-source-request-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: CreateDataSourceRequest
---
