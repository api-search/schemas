---
description: The output for the <a>DescribeConfigurationRecorderStatus</a> action, in JSON format.
layout: schema
name: DescribeConfigurationRecorderStatusResponse
properties_list:
- description: ''
  name: ConfigurationRecordersStatus
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-configuration-recorder-status-response-schema.json
slug: config-describe-configuration-recorder-status-response
source_filename: config-describe-configuration-recorder-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-configuration-recorder-status-response-schema.json\",\n  \"title\": \"DescribeConfigurationRecorderStatusResponse\",\n  \"description\": \"The output for the <a>DescribeConfigurationRecorderStatus</a> action, in JSON format.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationRecordersStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationRecorderStatusList\"\n        },\n        {\n          \"description\": \"A list that contains status of the specified recorders.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-configuration-recorder-status-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeConfigurationRecorderStatusResponse
---
