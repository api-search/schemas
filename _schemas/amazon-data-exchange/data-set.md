---
description: An AWS Data Exchange data set containing a collection of data available for subscription.
layout: schema
name: Data Set
properties_list:
- description: The unique identifier of the data set
  name: Id
  type: string
- description: The ARN of the data set
  name: Arn
  type: string
- description: The name of the data set
  name: Name
  type: string
- description: The description of the data set
  name: Description
  type: string
- description: ''
  name: AssetType
  type: string
- description: ''
  name: Origin
  type: string
- description: ''
  name: Tags
  type: object
- description: ''
  name: CreatedAt
  type: string
- description: ''
  name: UpdatedAt
  type: string
provider_name: Amazon Data Exchange
provider_slug: amazon-data-exchange
schema_file: json-schema/data-set-schema.json
slug: data-set
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-exchange/json-schema/data-set-schema.json\",\n  \"title\": \"Data Set\",\n  \"description\": \"An AWS Data Exchange data set containing a collection of data available for subscription.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the data set\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the data set\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the data set\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the data set\"\n    },\n    \"AssetType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"S3_SNAPSHOT\",\n        \"REDSHIFT_DATA_SHARE\",\n        \"API_GATEWAY_API\",\n        \"LAKE_FORMATION_DATA_PERMISSION\"\
  ,\n        \"S3_DATA_ACCESS\"\n      ]\n    },\n    \"Origin\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"OWNED\",\n        \"ENTITLED\"\n      ]\n    },\n    \"Tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"UpdatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-exchange/refs/heads/main/json-schema/data-set-schema.json
tags:
- AWS
- Data Exchange
- Data Marketplace
- Third-Party Data
- Analytics
- Subscriptions
title: Data Set
---
