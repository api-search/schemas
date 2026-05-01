---
description: DynamoDB data source configuration
layout: schema
name: DynamodbDataSourceConfig
properties_list:
- description: DynamoDB table name
  name: tableName
  type: string
- description: AWS Region
  name: awsRegion
  type: string
- description: Whether to use caller credentials
  name: useCallerCredentials
  type: boolean
- description: Delta sync configuration
  name: deltaSyncConfig
  type: object
- description: Whether versioning is enabled
  name: versioned
  type: boolean
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-dynamodb-data-source-config-schema.json
slug: appsync-dynamodb-data-source-config
source_filename: appsync-dynamodb-data-source-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-dynamodb-data-source-config-schema.json\",\n  \"title\": \"DynamodbDataSourceConfig\",\n  \"description\": \"DynamoDB data source configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tableName\": {\n      \"type\": \"string\",\n      \"description\": \"DynamoDB table name\"\n    },\n    \"awsRegion\": {\n      \"type\": \"string\",\n      \"description\": \"AWS Region\"\n    },\n    \"useCallerCredentials\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to use caller credentials\"\n    },\n    \"deltaSyncConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Delta sync configuration\"\n    },\n    \"versioned\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether versioning is enabled\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-dynamodb-data-source-config-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
title: DynamodbDataSourceConfig
---
