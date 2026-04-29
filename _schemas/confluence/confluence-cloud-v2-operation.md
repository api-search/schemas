---
description: ''
layout: schema
name: Operation
properties_list:
- description: The operation type.
  name: operation
  type: string
- description: The target type for the operation.
  name: targetType
  type: string
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-cloud-v2-operation-schema.json
slug: confluence-cloud-v2-operation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Operation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operation\": {\n      \"type\": \"string\",\n      \"description\": \"The operation type.\"\n    },\n    \"targetType\": {\n      \"type\": \"string\",\n      \"description\": \"The target type for the operation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-cloud-v2-operation-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: Operation
---
