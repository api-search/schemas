---
description: Request to update a data source
layout: schema
name: UpdateDataSourceRequest
properties_list:
- description: Updated description
  name: description
  type: string
- description: Data source type
  name: type
  type: string
- description: IAM role ARN
  name: serviceRoleArn
  type: string
- description: dynamodbConfig
  name: dynamodbConfig
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-update-data-source-request-schema.json
slug: appsync-update-data-source-request
source_filename: appsync-update-data-source-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-update-data-source-request-schema.json\",\n  \"title\": \"UpdateDataSourceRequest\",\n  \"description\": \"Request to update a data source\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Updated description\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Data source type\"\n    },\n    \"serviceRoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"IAM role ARN\"\n    },\n    \"dynamodbConfig\": {\n      \"type\": \"string\",\n      \"description\": \"dynamodbConfig\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-update-data-source-request-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
title: UpdateDataSourceRequest
---
