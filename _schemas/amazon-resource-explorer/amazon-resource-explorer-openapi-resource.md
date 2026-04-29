---
description: Resource schema from openapi
layout: schema
name: Resource
properties_list:
- description: The Amazon Resource Name (ARN) of the resource.
  name: Arn
  type: string
- description: The date and time the resource was last updated.
  name: LastReportedAt
  type: string
- description: The AWS account ID of the account that owns the resource.
  name: OwningAccountId
  type: string
- description: The AWS Region where the resource exists.
  name: Region
  type: string
- description: The type of the resource.
  name: ResourceType
  type: string
- description: The AWS service that owns the resource.
  name: Service
  type: string
provider_name: Amazon Resource Explorer
provider_slug: amazon-resource-explorer
schema_file: json-schema/amazon-resource-explorer-openapi-resource-schema.json
slug: amazon-resource-explorer-openapi-resource
source_filename: amazon-resource-explorer-openapi-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-resource-explorer/refs/heads/main/json-schema/amazon-resource-explorer-openapi-resource-schema.json\",\n  \"title\": \"Resource\",\n  \"description\": \"Resource schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the resource.\"\n    },\n    \"LastReportedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the resource was last updated.\"\n    },\n    \"OwningAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS account ID of the account that owns the resource.\"\n    },\n    \"Region\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS Region where the resource exists.\"\n    },\n    \"ResourceType\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The type of the resource.\"\n    },\n    \"Service\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS service that owns the resource.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-resource-explorer/refs/heads/main/json-schema/amazon-resource-explorer-openapi-resource-schema.json
tags:
- AWS
- Discovery
- Inventory
- Operations
- Resource Management
title: Resource
---
