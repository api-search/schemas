---
description: <p/>
layout: schema
name: DescribeConfigRulesResponse
properties_list:
- description: ''
  name: ConfigRules
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-config-rules-response-schema.json
slug: config-describe-config-rules-response
source_filename: config-describe-config-rules-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-config-rules-response-schema.json\",\n  \"title\": \"DescribeConfigRulesResponse\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRules\"\n        },\n        {\n          \"description\": \"The details about your Config rules.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The string that you use in a subsequent request to get the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-config-rules-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeConfigRulesResponse
---
