---
description: A revision of a data set, representing a snapshot of data at a point in time.
layout: schema
name: Revision
properties_list:
- description: ''
  name: Id
  type: string
- description: ''
  name: Arn
  type: string
- description: ''
  name: DataSetId
  type: string
- description: ''
  name: Comment
  type: string
- description: ''
  name: Finalized
  type: boolean
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
schema_file: json-schema/revision-schema.json
slug: revision
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-exchange/json-schema/revision-schema.json\",\n  \"title\": \"Revision\",\n  \"description\": \"A revision of a data set, representing a snapshot of data at a point in time.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\"\n    },\n    \"Arn\": {\n      \"type\": \"string\"\n    },\n    \"DataSetId\": {\n      \"type\": \"string\"\n    },\n    \"Comment\": {\n      \"type\": \"string\"\n    },\n    \"Finalized\": {\n      \"type\": \"boolean\"\n    },\n    \"Tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"UpdatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-exchange/refs/heads/main/json-schema/revision-schema.json
tags:
- AWS
- Data Exchange
- Data Marketplace
- Third-Party Data
- Analytics
- Subscriptions
title: Revision
---
