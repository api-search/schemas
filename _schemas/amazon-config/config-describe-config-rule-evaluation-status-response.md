---
description: <p/>
layout: schema
name: DescribeConfigRuleEvaluationStatusResponse
properties_list:
- description: ''
  name: ConfigRulesEvaluationStatus
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-config-rule-evaluation-status-response-schema.json
slug: config-describe-config-rule-evaluation-status-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-config-rule-evaluation-status-response-schema.json\",\n  \"title\": \"DescribeConfigRuleEvaluationStatusResponse\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRulesEvaluationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRuleEvaluationStatusList\"\n        },\n        {\n          \"description\": \"Status information about your Config managed rules.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The string that you use in a subsequent request to get the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-config-rule-evaluation-status-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeConfigRuleEvaluationStatusResponse
---
