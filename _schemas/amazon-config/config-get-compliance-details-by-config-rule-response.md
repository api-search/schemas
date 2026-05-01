---
description: <p/>
layout: schema
name: GetComplianceDetailsByConfigRuleResponse
properties_list:
- description: ''
  name: EvaluationResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-compliance-details-by-config-rule-response-schema.json
slug: config-get-compliance-details-by-config-rule-response
source_filename: config-get-compliance-details-by-config-rule-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-compliance-details-by-config-rule-response-schema.json\",\n  \"title\": \"GetComplianceDetailsByConfigRuleResponse\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EvaluationResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EvaluationResults\"\n        },\n        {\n          \"description\": \"Indicates whether the Amazon Web Services resource complies with the specified Config rule.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The string that you use in a subsequent request to get the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-compliance-details-by-config-rule-response-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: GetComplianceDetailsByConfigRuleResponse
---
