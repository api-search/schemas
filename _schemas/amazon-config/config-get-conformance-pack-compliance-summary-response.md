---
description: GetConformancePackComplianceSummaryResponse schema
layout: schema
name: GetConformancePackComplianceSummaryResponse
properties_list:
- description: ''
  name: ConformancePackComplianceSummaryList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-conformance-pack-compliance-summary-response-schema.json
slug: config-get-conformance-pack-compliance-summary-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-conformance-pack-compliance-summary-response-schema.json\",\n  \"title\": \"GetConformancePackComplianceSummaryResponse\",\n  \"description\": \"GetConformancePackComplianceSummaryResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConformancePackComplianceSummaryList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackComplianceSummaryList\"\n        },\n        {\n          \"description\": \"A list of <code>ConformancePackComplianceSummary</code> objects. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The nextToken string returned on a previous page that you use to get the next page of\
  \ results in a paginated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-conformance-pack-compliance-summary-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: GetConformancePackComplianceSummaryResponse
---
