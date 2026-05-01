---
description: The output for the <a>DescribeConfigurationRecorders</a> action.
layout: schema
name: DescribeConfigurationRecordersResponse
properties_list:
- description: ''
  name: ConfigurationRecorders
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-configuration-recorders-response-schema.json
slug: config-describe-configuration-recorders-response
source_filename: config-describe-configuration-recorders-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-configuration-recorders-response-schema.json\",\n  \"title\": \"DescribeConfigurationRecordersResponse\",\n  \"description\": \"The output for the <a>DescribeConfigurationRecorders</a> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationRecorders\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationRecorderList\"\n        },\n        {\n          \"description\": \"A list that contains the descriptions of the specified configuration recorders.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-configuration-recorders-response-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeConfigurationRecordersResponse
---
