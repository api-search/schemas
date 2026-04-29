---
description: Index schema from openapi
layout: schema
name: Index
properties_list:
- description: The ARN of the index.
  name: Arn
  type: string
- description: The AWS Region where the index exists.
  name: Region
  type: string
- description: The type of the index.
  name: Type
  type: string
provider_name: Amazon Resource Explorer
provider_slug: amazon-resource-explorer
schema_file: json-schema/amazon-resource-explorer-openapi-index-schema.json
slug: amazon-resource-explorer-openapi-index
source_filename: amazon-resource-explorer-openapi-index-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-resource-explorer/refs/heads/main/json-schema/amazon-resource-explorer-openapi-index-schema.json\",\n  \"title\": \"Index\",\n  \"description\": \"Index schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the index.\"\n    },\n    \"Region\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS Region where the index exists.\"\n    },\n    \"Type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"LOCAL\",\n        \"AGGREGATOR\"\n      ],\n      \"description\": \"The type of the index.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-resource-explorer/refs/heads/main/json-schema/amazon-resource-explorer-openapi-index-schema.json
tags:
- AWS
- Discovery
- Inventory
- Operations
- Resource Management
title: Index
---
