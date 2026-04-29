---
description: A data source configuration for a GraphQL API
layout: schema
name: DataSource
properties_list:
- description: The ARN of the data source
  name: dataSourceArn
  type: string
- description: The data source name
  name: name
  type: string
- description: The data source description
  name: description
  type: string
- description: The data source type
  name: type
  type: string
- description: IAM service role ARN
  name: serviceRoleArn
  type: string
- description: dynamodbConfig
  name: dynamodbConfig
  type: string
- description: lambdaConfig
  name: lambdaConfig
  type: string
- description: elasticsearchConfig
  name: elasticsearchConfig
  type: string
- description: httpConfig
  name: httpConfig
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-data-source-schema.json
slug: appsync-data-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-data-source-schema.json\",\n  \"title\": \"DataSource\",\n  \"description\": \"A data source configuration for a GraphQL API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dataSourceArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the data source\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The data source name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The data source description\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The data source type\"\n    },\n    \"serviceRoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"IAM service role ARN\"\n    },\n    \"dynamodbConfig\": {\n      \"type\": \"string\",\n      \"description\": \"dynamodbConfig\"\n    },\n \
  \   \"lambdaConfig\": {\n      \"type\": \"string\",\n      \"description\": \"lambdaConfig\"\n    },\n    \"elasticsearchConfig\": {\n      \"type\": \"string\",\n      \"description\": \"elasticsearchConfig\"\n    },\n    \"httpConfig\": {\n      \"type\": \"string\",\n      \"description\": \"httpConfig\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-data-source-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: DataSource
---
