---
description: ''
layout: schema
name: ItemCollectionMetrics
properties_list:
- description: The partition key value of the item collection
  name: ItemCollectionKey
  type: object
- description: An estimate of item collection size in gigabytes
  name: SizeEstimateRangeGB
  type: array
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-item-collection-metrics-schema.json
slug: dynamodb-item-collection-metrics
source_filename: dynamodb-item-collection-metrics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ItemCollectionMetrics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ItemCollectionKey\": {\n      \"type\": \"object\",\n      \"description\": \"The partition key value of the item collection\"\n    },\n    \"SizeEstimateRangeGB\": {\n      \"type\": \"array\",\n      \"description\": \"An estimate of item collection size in gigabytes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-item-collection-metrics-schema.json
tags:
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: ItemCollectionMetrics
---
