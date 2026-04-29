---
description: DeleteConfigurationAggregatorRequest schema
layout: schema
name: DeleteConfigurationAggregatorRequest
properties_list:
- description: ''
  name: ConfigurationAggregatorName
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-delete-configuration-aggregator-request-schema.json
slug: config-delete-configuration-aggregator-request
source_filename: config-delete-configuration-aggregator-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-configuration-aggregator-request-schema.json\",\n  \"title\": \"DeleteConfigurationAggregatorRequest\",\n  \"description\": \"DeleteConfigurationAggregatorRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationAggregatorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationAggregatorName\"\n        },\n        {\n          \"description\": \"The name of the configuration aggregator.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigurationAggregatorName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-configuration-aggregator-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DeleteConfigurationAggregatorRequest
---
