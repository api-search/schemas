---
description: GetAggregateResourceConfigResponse schema
layout: schema
name: GetAggregateResourceConfigResponse
properties_list:
- description: ''
  name: ConfigurationItem
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-aggregate-resource-config-response-schema.json
slug: config-get-aggregate-resource-config-response
source_filename: config-get-aggregate-resource-config-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-aggregate-resource-config-response-schema.json\",\n  \"title\": \"GetAggregateResourceConfigResponse\",\n  \"description\": \"GetAggregateResourceConfigResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationItem\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationItem\"\n        },\n        {\n          \"description\": \"Returns a <code>ConfigurationItem</code> object.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-aggregate-resource-config-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: GetAggregateResourceConfigResponse
---
