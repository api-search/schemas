---
description: Summary includes the name and status of the conformance pack.
layout: schema
name: ConformancePackComplianceSummary
properties_list:
- description: ''
  name: ConformancePackName
  type: object
- description: ''
  name: ConformancePackComplianceStatus
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-conformance-pack-compliance-summary-schema.json
slug: config-conformance-pack-compliance-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-compliance-summary-schema.json\",\n  \"title\": \"ConformancePackComplianceSummary\",\n  \"description\": \"Summary includes the name and status of the conformance pack.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConformancePackName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackName\"\n        },\n        {\n          \"description\": \"The name of the conformance pack name.\"\n        }\n      ]\n    },\n    \"ConformancePackComplianceStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackComplianceType\"\n        },\n        {\n          \"description\": \"The status of the conformance pack.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConformancePackName\"\
  ,\n    \"ConformancePackComplianceStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-compliance-summary-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ConformancePackComplianceSummary
---
