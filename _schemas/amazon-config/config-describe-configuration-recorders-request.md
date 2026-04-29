---
description: The input for the <a>DescribeConfigurationRecorders</a> action.
layout: schema
name: DescribeConfigurationRecordersRequest
properties_list:
- description: ''
  name: ConfigurationRecorderNames
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-configuration-recorders-request-schema.json
slug: config-describe-configuration-recorders-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-configuration-recorders-request-schema.json\",\n  \"title\": \"DescribeConfigurationRecordersRequest\",\n  \"description\": \"The input for the <a>DescribeConfigurationRecorders</a> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationRecorderNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationRecorderNameList\"\n        },\n        {\n          \"description\": \"A list of configuration recorder names.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-configuration-recorders-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeConfigurationRecordersRequest
---
