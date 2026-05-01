---
description: SearchResponse schema from openapi
layout: schema
name: SearchResponse
properties_list:
- description: The count of matching resources.
  name: Count
  type: object
- description: The token for the next page of results.
  name: NextToken
  type: string
- description: ''
  name: Resources
  type: array
- description: The ARN of the view used for the search.
  name: ViewArn
  type: string
provider_name: Amazon Resource Explorer
provider_slug: amazon-resource-explorer
schema_file: json-schema/amazon-resource-explorer-openapi-search-response-schema.json
slug: amazon-resource-explorer-openapi-search-response
source_filename: amazon-resource-explorer-openapi-search-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-resource-explorer/refs/heads/main/json-schema/amazon-resource-explorer-openapi-search-response-schema.json\",\n  \"title\": \"SearchResponse\",\n  \"description\": \"SearchResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Count\": {\n      \"type\": \"object\",\n      \"description\": \"The count of matching resources.\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token for the next page of results.\"\n    },\n    \"Resources\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Resource\"\n      }\n    },\n    \"ViewArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the view used for the search.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-resource-explorer/refs/heads/main/json-schema/amazon-resource-explorer-openapi-search-response-schema.json
tags:
- Discovery
- Inventory
- Operations
- Resource Management
title: SearchResponse
---
