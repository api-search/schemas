---
description: GetAggregateConfigRuleComplianceSummaryResponse schema
layout: schema
name: GetAggregateConfigRuleComplianceSummaryResponse
properties_list:
- description: ''
  name: GroupByKey
  type: object
- description: ''
  name: AggregateComplianceCounts
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-aggregate-config-rule-compliance-summary-response-schema.json
slug: config-get-aggregate-config-rule-compliance-summary-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-aggregate-config-rule-compliance-summary-response-schema.json\",\n  \"title\": \"GetAggregateConfigRuleComplianceSummaryResponse\",\n  \"description\": \"GetAggregateConfigRuleComplianceSummaryResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GroupByKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"Groups the result based on ACCOUNT_ID or AWS_REGION.\"\n        }\n      ]\n    },\n    \"AggregateComplianceCounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregateComplianceCountList\"\n        },\n        {\n          \"description\": \"Returns a list of AggregateComplianceCounts object.\"\n        }\n      ]\n    },\n    \"\
  NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-aggregate-config-rule-compliance-summary-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: GetAggregateConfigRuleComplianceSummaryResponse
---
