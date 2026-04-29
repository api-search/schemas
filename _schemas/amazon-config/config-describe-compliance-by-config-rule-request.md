---
description: <p/>
layout: schema
name: DescribeComplianceByConfigRuleRequest
properties_list:
- description: ''
  name: ConfigRuleNames
  type: object
- description: ''
  name: ComplianceTypes
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-compliance-by-config-rule-request-schema.json
slug: config-describe-compliance-by-config-rule-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-compliance-by-config-rule-request-schema.json\",\n  \"title\": \"DescribeComplianceByConfigRuleRequest\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRuleNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRuleNames\"\n        },\n        {\n          \"description\": \"Specify one or more Config rule names to filter the results by rule.\"\n        }\n      ]\n    },\n    \"ComplianceTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComplianceTypes\"\n        },\n        {\n          \"description\": \"Filters the results by compliance.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\
  \n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-compliance-by-config-rule-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeComplianceByConfigRuleRequest
---
