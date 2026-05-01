---
description: Filters the compliance results based on account ID, region, compliance type, and rule name.
layout: schema
name: ConfigRuleComplianceFilters
properties_list:
- description: ''
  name: ConfigRuleName
  type: object
- description: ''
  name: ComplianceType
  type: object
- description: ''
  name: AccountId
  type: object
- description: ''
  name: AwsRegion
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-config-rule-compliance-filters-schema.json
slug: config-config-rule-compliance-filters
source_filename: config-config-rule-compliance-filters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-config-rule-compliance-filters-schema.json\",\n  \"title\": \"ConfigRuleComplianceFilters\",\n  \"description\": \"Filters the compliance results based on account ID, region, compliance type, and rule name.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRuleName\"\n        },\n        {\n          \"description\": \"The name of the Config rule.\"\n        }\n      ]\n    },\n    \"ComplianceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComplianceType\"\n        },\n        {\n          \"description\": \"<p>The rule compliance status.</p> <p>For the <code>ConfigRuleComplianceFilters</code> data type, Config supports only <code>COMPLIANT</code> and <code>NON_COMPLIANT</code>.\
  \ Config does not support the <code>NOT_APPLICABLE</code> and the <code>INSUFFICIENT_DATA</code> values.</p>\"\n        }\n      ]\n    },\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The 12-digit account ID of the source account. \"\n        }\n      ]\n    },\n    \"AwsRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsRegion\"\n        },\n        {\n          \"description\": \"The source region where the data is aggregated. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-config-rule-compliance-filters-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: ConfigRuleComplianceFilters
---
