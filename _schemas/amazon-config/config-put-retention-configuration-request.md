---
description: PutRetentionConfigurationRequest schema
layout: schema
name: PutRetentionConfigurationRequest
properties_list:
- description: ''
  name: RetentionPeriodInDays
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-retention-configuration-request-schema.json
slug: config-put-retention-configuration-request
source_filename: config-put-retention-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-retention-configuration-request-schema.json\",\n  \"title\": \"PutRetentionConfigurationRequest\",\n  \"description\": \"PutRetentionConfigurationRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RetentionPeriodInDays\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RetentionPeriodInDays\"\n        },\n        {\n          \"description\": \"<p>Number of days Config stores your historical information.</p> <note> <p>Currently, only applicable to the configuration item history.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RetentionPeriodInDays\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-retention-configuration-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: PutRetentionConfigurationRequest
---
