---
description: The dynamic value of the resource.
layout: schema
name: ResourceValue
properties_list:
- description: ''
  name: Value
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-resource-value-schema.json
slug: config-resource-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-resource-value-schema.json\",\n  \"title\": \"ResourceValue\",\n  \"description\": \"The dynamic value of the resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceValueType\"\n        },\n        {\n          \"description\": \"The value is a resource ID.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-resource-value-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ResourceValue
---
