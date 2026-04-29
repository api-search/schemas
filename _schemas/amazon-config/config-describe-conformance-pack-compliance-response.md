---
description: DescribeConformancePackComplianceResponse schema
layout: schema
name: DescribeConformancePackComplianceResponse
properties_list:
- description: ''
  name: ConformancePackName
  type: object
- description: ''
  name: ConformancePackRuleComplianceList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-conformance-pack-compliance-response-schema.json
slug: config-describe-conformance-pack-compliance-response
source_filename: config-describe-conformance-pack-compliance-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-conformance-pack-compliance-response-schema.json\",\n  \"title\": \"DescribeConformancePackComplianceResponse\",\n  \"description\": \"DescribeConformancePackComplianceResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConformancePackName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackName\"\n        },\n        {\n          \"description\": \"Name of the conformance pack.\"\n        }\n      ]\n    },\n    \"ConformancePackRuleComplianceList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackRuleComplianceList\"\n        },\n        {\n          \"description\": \"Returns a list of <code>ConformancePackRuleCompliance</code> objects.\"\n        }\n      ]\n    },\n    \"NextToken\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned in a previous request that you use to request the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConformancePackName\",\n    \"ConformancePackRuleComplianceList\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-conformance-pack-compliance-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeConformancePackComplianceResponse
---
