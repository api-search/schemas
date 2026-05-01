---
description: PutRetentionConfigurationResponse schema
layout: schema
name: PutRetentionConfigurationResponse
properties_list:
- description: ''
  name: RetentionConfiguration
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-retention-configuration-response-schema.json
slug: config-put-retention-configuration-response
source_filename: config-put-retention-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-retention-configuration-response-schema.json\",\n  \"title\": \"PutRetentionConfigurationResponse\",\n  \"description\": \"PutRetentionConfigurationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RetentionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RetentionConfiguration\"\n        },\n        {\n          \"description\": \"Returns a retention configuration object.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-retention-configuration-response-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: PutRetentionConfigurationResponse
---
