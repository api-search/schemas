---
description: BatchGetResourceConfigResponse schema
layout: schema
name: BatchGetResourceConfigResponse
properties_list:
- description: ''
  name: baseConfigurationItems
  type: object
- description: ''
  name: unprocessedResourceKeys
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-batch-get-resource-config-response-schema.json
slug: config-batch-get-resource-config-response
source_filename: config-batch-get-resource-config-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-batch-get-resource-config-response-schema.json\",\n  \"title\": \"BatchGetResourceConfigResponse\",\n  \"description\": \"BatchGetResourceConfigResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"baseConfigurationItems\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BaseConfigurationItems\"\n        },\n        {\n          \"description\": \"A list that contains the current configuration of one or more resources.\"\n        }\n      ]\n    },\n    \"unprocessedResourceKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceKeys\"\n        },\n        {\n          \"description\": \"A list of resource keys that were not processed with the current response. The unprocessesResourceKeys value is in the same form\
  \ as ResourceKeys, so the value can be directly provided to a subsequent BatchGetResourceConfig operation. If there are no unprocessed resource keys, the response contains an empty unprocessedResourceKeys list. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-batch-get-resource-config-response-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: BatchGetResourceConfigResponse
---
