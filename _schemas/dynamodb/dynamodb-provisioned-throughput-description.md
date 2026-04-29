---
description: ''
layout: schema
name: ProvisionedThroughputDescription
properties_list:
- description: The date and time of the last provisioned throughput increase
  name: LastIncreaseDateTime
  type: string
- description: The date and time of the last provisioned throughput decrease
  name: LastDecreaseDateTime
  type: string
- description: The number of provisioned throughput decreases for this table during this UTC calendar day
  name: NumberOfDecreasesToday
  type: integer
- description: The maximum number of strongly consistent reads consumed per second
  name: ReadCapacityUnits
  type: integer
- description: The maximum number of writes consumed per second
  name: WriteCapacityUnits
  type: integer
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-provisioned-throughput-description-schema.json
slug: dynamodb-provisioned-throughput-description
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProvisionedThroughputDescription\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LastIncreaseDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time of the last provisioned throughput increase\"\n    },\n    \"LastDecreaseDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time of the last provisioned throughput decrease\"\n    },\n    \"NumberOfDecreasesToday\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of provisioned throughput decreases for this table during this UTC calendar day\"\n    },\n    \"ReadCapacityUnits\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of strongly consistent reads consumed per second\"\n    },\n    \"WriteCapacityUnits\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of writes consumed per second\"\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-provisioned-throughput-description-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: ProvisionedThroughputDescription
---
