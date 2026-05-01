---
description: DeleteResourceConfigRequest schema
layout: schema
name: DeleteResourceConfigRequest
properties_list:
- description: ''
  name: ResourceType
  type: object
- description: ''
  name: ResourceId
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-delete-resource-config-request-schema.json
slug: config-delete-resource-config-request
source_filename: config-delete-resource-config-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-resource-config-request-schema.json\",\n  \"title\": \"DeleteResourceConfigRequest\",\n  \"description\": \"DeleteResourceConfigRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceTypeString\"\n        },\n        {\n          \"description\": \"The type of the resource.\"\n        }\n      ]\n    },\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"Unique identifier of the resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceType\",\n    \"ResourceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-resource-config-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: DeleteResourceConfigRequest
---
