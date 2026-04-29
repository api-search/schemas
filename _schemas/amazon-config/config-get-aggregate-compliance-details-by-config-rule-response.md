---
description: GetAggregateComplianceDetailsByConfigRuleResponse schema
layout: schema
name: GetAggregateComplianceDetailsByConfigRuleResponse
properties_list:
- description: ''
  name: AggregateEvaluationResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-aggregate-compliance-details-by-config-rule-response-schema.json
slug: config-get-aggregate-compliance-details-by-config-rule-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-aggregate-compliance-details-by-config-rule-response-schema.json\",\n  \"title\": \"GetAggregateComplianceDetailsByConfigRuleResponse\",\n  \"description\": \"GetAggregateComplianceDetailsByConfigRuleResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AggregateEvaluationResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregateEvaluationResultList\"\n        },\n        {\n          \"description\": \"Returns an AggregateEvaluationResults object.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results\
  \ in a paginated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-aggregate-compliance-details-by-config-rule-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: GetAggregateComplianceDetailsByConfigRuleResponse
---
