---
description: Describes the provisioned throughput settings for a table or index
layout: schema
name: ProvisionedThroughputDescription
properties_list:
- description: The date and time of the last provisioned throughput increase
  name: LastIncreaseDateTime
  type: number
- description: The date and time of the last provisioned throughput decrease
  name: LastDecreaseDateTime
  type: number
- description: The number of provisioned throughput decreases for this table during this UTC calendar day
  name: NumberOfDecreasesToday
  type: integer
- description: The maximum number of strongly consistent reads per second
  name: ReadCapacityUnits
  type: integer
- description: The maximum number of writes per second
  name: WriteCapacityUnits
  type: integer
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-provisioned-throughput-description-schema.json
slug: dynamodb-openapi-provisioned-throughput-description
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-provisioned-throughput-description-schema.json\",\n  \"title\": \"ProvisionedThroughputDescription\",\n  \"description\": \"Describes the provisioned throughput settings for a table or index\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LastIncreaseDateTime\": {\n      \"type\": \"number\",\n      \"description\": \"The date and time of the last provisioned throughput increase\"\n    },\n    \"LastDecreaseDateTime\": {\n      \"type\": \"number\",\n      \"description\": \"The date and time of the last provisioned throughput decrease\"\n    },\n    \"NumberOfDecreasesToday\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of provisioned throughput decreases for this table during this UTC calendar day\"\n    },\n    \"ReadCapacityUnits\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"The maximum number of strongly consistent reads per second\"\n    },\n    \"WriteCapacityUnits\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of writes per second\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-provisioned-throughput-description-schema.json
tags:
- AWS
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: ProvisionedThroughputDescription
---
