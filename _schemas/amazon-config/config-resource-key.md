---
description: The details that identify a resource within Config, including the resource type and resource ID.
layout: schema
name: ResourceKey
properties_list:
- description: ''
  name: resourceType
  type: object
- description: ''
  name: resourceId
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-resource-key-schema.json
slug: config-resource-key
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-resource-key-schema.json\",\n  \"title\": \"ResourceKey\",\n  \"description\": \"The details that identify a resource within Config, including the resource type and resource ID.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceType\"\n        },\n        {\n          \"description\": \"The resource type.\"\n        }\n      ]\n    },\n    \"resourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the resource (for example., sg-xxxxxx). \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceType\",\n    \"resourceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-resource-key-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ResourceKey
---
