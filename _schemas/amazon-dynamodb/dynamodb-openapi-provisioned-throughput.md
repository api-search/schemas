---
description: Represents the provisioned throughput settings for a table or index
layout: schema
name: ProvisionedThroughput
properties_list:
- description: The maximum number of strongly consistent reads per second
  name: ReadCapacityUnits
  type: integer
- description: The maximum number of writes per second
  name: WriteCapacityUnits
  type: integer
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-provisioned-throughput-schema.json
slug: dynamodb-openapi-provisioned-throughput
source_filename: dynamodb-openapi-provisioned-throughput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-provisioned-throughput-schema.json\",\n  \"title\": \"ProvisionedThroughput\",\n  \"description\": \"Represents the provisioned throughput settings for a table or index\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReadCapacityUnits\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of strongly consistent reads per second\",\n      \"minimum\": 1\n    },\n    \"WriteCapacityUnits\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of writes per second\",\n      \"minimum\": 1\n    }\n  },\n  \"required\": [\n    \"ReadCapacityUnits\",\n    \"WriteCapacityUnits\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-provisioned-throughput-schema.json
tags:
- AWS
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: ProvisionedThroughput
---
