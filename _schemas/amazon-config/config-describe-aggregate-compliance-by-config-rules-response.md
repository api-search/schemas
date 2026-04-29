---
description: DescribeAggregateComplianceByConfigRulesResponse schema
layout: schema
name: DescribeAggregateComplianceByConfigRulesResponse
properties_list:
- description: ''
  name: AggregateComplianceByConfigRules
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-aggregate-compliance-by-config-rules-response-schema.json
slug: config-describe-aggregate-compliance-by-config-rules-response
source_filename: config-describe-aggregate-compliance-by-config-rules-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-aggregate-compliance-by-config-rules-response-schema.json\",\n  \"title\": \"DescribeAggregateComplianceByConfigRulesResponse\",\n  \"description\": \"DescribeAggregateComplianceByConfigRulesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AggregateComplianceByConfigRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregateComplianceByConfigRuleList\"\n        },\n        {\n          \"description\": \"Returns a list of AggregateComplianceByConfigRule object.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get\
  \ the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-aggregate-compliance-by-config-rules-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeAggregateComplianceByConfigRulesResponse
---
