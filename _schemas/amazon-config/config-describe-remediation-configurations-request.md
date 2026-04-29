---
description: DescribeRemediationConfigurationsRequest schema
layout: schema
name: DescribeRemediationConfigurationsRequest
properties_list:
- description: ''
  name: ConfigRuleNames
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-remediation-configurations-request-schema.json
slug: config-describe-remediation-configurations-request
source_filename: config-describe-remediation-configurations-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-remediation-configurations-request-schema.json\",\n  \"title\": \"DescribeRemediationConfigurationsRequest\",\n  \"description\": \"DescribeRemediationConfigurationsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRuleNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRuleNames\"\n        },\n        {\n          \"description\": \"A list of Config rule names of remediation configurations for which you want details. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigRuleNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-remediation-configurations-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeRemediationConfigurationsRequest
---
