---
description: View schema from openapi
layout: schema
name: View
properties_list:
- description: The filters applied to the view.
  name: Filters
  type: object
- description: Additional properties to include in the view.
  name: IncludedProperties
  type: array
- description: The ARN of the view.
  name: ViewArn
  type: string
provider_name: Amazon Resource Explorer
provider_slug: amazon-resource-explorer
schema_file: json-schema/amazon-resource-explorer-openapi-view-schema.json
slug: amazon-resource-explorer-openapi-view
source_filename: amazon-resource-explorer-openapi-view-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-resource-explorer/refs/heads/main/json-schema/amazon-resource-explorer-openapi-view-schema.json\",\n  \"title\": \"View\",\n  \"description\": \"View schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Filters\": {\n      \"type\": \"object\",\n      \"description\": \"The filters applied to the view.\"\n    },\n    \"IncludedProperties\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"Additional properties to include in the view.\"\n    },\n    \"ViewArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the view.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-resource-explorer/refs/heads/main/json-schema/amazon-resource-explorer-openapi-view-schema.json
tags:
- AWS
- Discovery
- Inventory
- Operations
- Resource Management
title: View
---
