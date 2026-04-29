---
description: BatchGetResourceConfigRequest schema
layout: schema
name: BatchGetResourceConfigRequest
properties_list:
- description: ''
  name: resourceKeys
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-batch-get-resource-config-request-schema.json
slug: config-batch-get-resource-config-request
source_filename: config-batch-get-resource-config-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-batch-get-resource-config-request-schema.json\",\n  \"title\": \"BatchGetResourceConfigRequest\",\n  \"description\": \"BatchGetResourceConfigRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceKeys\"\n        },\n        {\n          \"description\": \"A list of resource keys to be processed with the current request. Each element in the list consists of the resource type and resource ID.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceKeys\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-batch-get-resource-config-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: BatchGetResourceConfigRequest
---
