---
description: DeleteRetentionConfigurationRequest schema
layout: schema
name: DeleteRetentionConfigurationRequest
properties_list:
- description: ''
  name: RetentionConfigurationName
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-delete-retention-configuration-request-schema.json
slug: config-delete-retention-configuration-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-retention-configuration-request-schema.json\",\n  \"title\": \"DeleteRetentionConfigurationRequest\",\n  \"description\": \"DeleteRetentionConfigurationRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RetentionConfigurationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RetentionConfigurationName\"\n        },\n        {\n          \"description\": \"The name of the retention configuration to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RetentionConfigurationName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-retention-configuration-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DeleteRetentionConfigurationRequest
---
