---
description: The input for the <a>DescribeConfigurationRecorderStatus</a> action.
layout: schema
name: DescribeConfigurationRecorderStatusRequest
properties_list:
- description: ''
  name: ConfigurationRecorderNames
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-configuration-recorder-status-request-schema.json
slug: config-describe-configuration-recorder-status-request
source_filename: config-describe-configuration-recorder-status-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-configuration-recorder-status-request-schema.json\",\n  \"title\": \"DescribeConfigurationRecorderStatusRequest\",\n  \"description\": \"The input for the <a>DescribeConfigurationRecorderStatus</a> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationRecorderNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationRecorderNameList\"\n        },\n        {\n          \"description\": \"The name(s) of the configuration recorder. If the name is not specified, the action returns the current status of all the configuration recorders associated with the account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-configuration-recorder-status-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeConfigurationRecorderStatusRequest
---
