---
description: An object with the name of the retention configuration and the retention period in days. The object stores the configuration for data retention in Config.
layout: schema
name: RetentionConfiguration
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: RetentionPeriodInDays
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-retention-configuration-schema.json
slug: config-retention-configuration
source_filename: config-retention-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-retention-configuration-schema.json\",\n  \"title\": \"RetentionConfiguration\",\n  \"description\": \"An object with the name of the retention configuration and the retention period in days. The object stores the configuration for data retention in Config.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RetentionConfigurationName\"\n        },\n        {\n          \"description\": \"The name of the retention configuration object.\"\n        }\n      ]\n    },\n    \"RetentionPeriodInDays\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RetentionPeriodInDays\"\n        },\n        {\n          \"description\": \"<p>Number of days Config stores your historical information.</p>\
  \ <note> <p>Currently, only applicable to the configuration item history.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"RetentionPeriodInDays\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-retention-configuration-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: RetentionConfiguration
---
