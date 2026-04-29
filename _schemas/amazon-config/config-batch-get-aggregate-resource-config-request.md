---
description: BatchGetAggregateResourceConfigRequest schema
layout: schema
name: BatchGetAggregateResourceConfigRequest
properties_list:
- description: ''
  name: ConfigurationAggregatorName
  type: object
- description: ''
  name: ResourceIdentifiers
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-batch-get-aggregate-resource-config-request-schema.json
slug: config-batch-get-aggregate-resource-config-request
source_filename: config-batch-get-aggregate-resource-config-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-batch-get-aggregate-resource-config-request-schema.json\",\n  \"title\": \"BatchGetAggregateResourceConfigRequest\",\n  \"description\": \"BatchGetAggregateResourceConfigRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationAggregatorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationAggregatorName\"\n        },\n        {\n          \"description\": \"The name of the configuration aggregator.\"\n        }\n      ]\n    },\n    \"ResourceIdentifiers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdentifiersList\"\n        },\n        {\n          \"description\": \"A list of aggregate ResourceIdentifiers objects. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigurationAggregatorName\"\
  ,\n    \"ResourceIdentifiers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-batch-get-aggregate-resource-config-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: BatchGetAggregateResourceConfigRequest
---
