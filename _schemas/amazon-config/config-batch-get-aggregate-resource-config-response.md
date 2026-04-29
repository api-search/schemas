---
description: BatchGetAggregateResourceConfigResponse schema
layout: schema
name: BatchGetAggregateResourceConfigResponse
properties_list:
- description: ''
  name: BaseConfigurationItems
  type: object
- description: ''
  name: UnprocessedResourceIdentifiers
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-batch-get-aggregate-resource-config-response-schema.json
slug: config-batch-get-aggregate-resource-config-response
source_filename: config-batch-get-aggregate-resource-config-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-batch-get-aggregate-resource-config-response-schema.json\",\n  \"title\": \"BatchGetAggregateResourceConfigResponse\",\n  \"description\": \"BatchGetAggregateResourceConfigResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BaseConfigurationItems\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BaseConfigurationItems\"\n        },\n        {\n          \"description\": \"A list that contains the current configuration of one or more resources.\"\n        }\n      ]\n    },\n    \"UnprocessedResourceIdentifiers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnprocessedResourceIdentifierList\"\n        },\n        {\n          \"description\": \"A list of resource identifiers that were not processed with current scope.\
  \ The list is empty if all the resources are processed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-batch-get-aggregate-resource-config-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: BatchGetAggregateResourceConfigResponse
---
