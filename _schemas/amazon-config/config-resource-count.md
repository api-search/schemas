---
description: An object that contains the resource type and the number of resources.
layout: schema
name: ResourceCount
properties_list:
- description: ''
  name: resourceType
  type: object
- description: ''
  name: count
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-resource-count-schema.json
slug: config-resource-count
source_filename: config-resource-count-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-resource-count-schema.json\",\n  \"title\": \"ResourceCount\",\n  \"description\": \"An object that contains the resource type and the number of resources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceType\"\n        },\n        {\n          \"description\": \"The resource type (for example, <code>\\\"AWS::EC2::Instance\\\"</code>).\"\n        }\n      ]\n    },\n    \"count\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The number of resources.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-resource-count-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: ResourceCount
---
