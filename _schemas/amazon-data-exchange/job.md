---
description: A Data Exchange job for importing or exporting assets.
layout: schema
name: Job
properties_list:
- description: ''
  name: Id
  type: string
- description: ''
  name: Arn
  type: string
- description: ''
  name: Type
  type: string
- description: ''
  name: State
  type: string
- description: ''
  name: Details
  type: object
- description: ''
  name: Errors
  type: array
- description: ''
  name: CreatedAt
  type: string
- description: ''
  name: UpdatedAt
  type: string
provider_name: Amazon Data Exchange
provider_slug: amazon-data-exchange
schema_file: json-schema/job-schema.json
slug: job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-exchange/json-schema/job-schema.json\",\n  \"title\": \"Job\",\n  \"description\": \"A Data Exchange job for importing or exporting assets.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\"\n    },\n    \"Arn\": {\n      \"type\": \"string\"\n    },\n    \"Type\": {\n      \"type\": \"string\"\n    },\n    \"State\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"WAITING\",\n        \"IN_PROGRESS\",\n        \"ERROR\",\n        \"COMPLETED\",\n        \"CANCELLED\",\n        \"TIMED_OUT\"\n      ]\n    },\n    \"Details\": {\n      \"type\": \"object\"\n    },\n    \"Errors\": {\n      \"type\": \"array\"\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"UpdatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-exchange/refs/heads/main/json-schema/job-schema.json
tags:
- AWS
- Data Exchange
- Data Marketplace
- Third-Party Data
- Analytics
- Subscriptions
title: Job
---
