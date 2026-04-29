---
description: <p/>
layout: schema
name: GetComplianceSummaryByConfigRuleResponse
properties_list:
- description: ''
  name: ComplianceSummary
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-compliance-summary-by-config-rule-response-schema.json
slug: config-get-compliance-summary-by-config-rule-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-compliance-summary-by-config-rule-response-schema.json\",\n  \"title\": \"GetComplianceSummaryByConfigRuleResponse\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ComplianceSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComplianceSummary\"\n        },\n        {\n          \"description\": \"The number of Config rules that are compliant and the number that are noncompliant, up to a maximum of 25 for each.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-compliance-summary-by-config-rule-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: GetComplianceSummaryByConfigRuleResponse
---
