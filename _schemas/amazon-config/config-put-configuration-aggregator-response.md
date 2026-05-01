---
description: PutConfigurationAggregatorResponse schema
layout: schema
name: PutConfigurationAggregatorResponse
properties_list:
- description: ''
  name: ConfigurationAggregator
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-configuration-aggregator-response-schema.json
slug: config-put-configuration-aggregator-response
source_filename: config-put-configuration-aggregator-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-configuration-aggregator-response-schema.json\",\n  \"title\": \"PutConfigurationAggregatorResponse\",\n  \"description\": \"PutConfigurationAggregatorResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationAggregator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationAggregator\"\n        },\n        {\n          \"description\": \"Returns a ConfigurationAggregator object.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-configuration-aggregator-response-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: PutConfigurationAggregatorResponse
---
