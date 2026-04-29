---
description: ''
layout: schema
name: ProvisionedThroughput
properties_list:
- description: The maximum number of strongly consistent reads consumed per second
  name: ReadCapacityUnits
  type: integer
- description: The maximum number of writes consumed per second
  name: WriteCapacityUnits
  type: integer
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-provisioned-throughput-schema.json
slug: dynamodb-provisioned-throughput
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProvisionedThroughput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReadCapacityUnits\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of strongly consistent reads consumed per second\"\n    },\n    \"WriteCapacityUnits\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of writes consumed per second\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-provisioned-throughput-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: ProvisionedThroughput
---
