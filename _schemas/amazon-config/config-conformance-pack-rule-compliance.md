---
description: Compliance information of one or more Config rules within a conformance pack. You can filter using Config rule names and compliance types.
layout: schema
name: ConformancePackRuleCompliance
properties_list:
- description: ''
  name: ConfigRuleName
  type: object
- description: ''
  name: ComplianceType
  type: object
- description: ''
  name: Controls
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-conformance-pack-rule-compliance-schema.json
slug: config-conformance-pack-rule-compliance
source_filename: config-conformance-pack-rule-compliance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-rule-compliance-schema.json\",\n  \"title\": \"ConformancePackRuleCompliance\",\n  \"description\": \"Compliance information of one or more Config rules within a conformance pack. You can filter using Config rule names and compliance types.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRuleName\"\n        },\n        {\n          \"description\": \"Name of the Config rule.\"\n        }\n      ]\n    },\n    \"ComplianceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackComplianceType\"\n        },\n        {\n          \"description\": \"Compliance of the Config rule.\"\n        }\n      ]\n    },\n    \"Controls\": {\n   \
  \   \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ControlsList\"\n        },\n        {\n          \"description\": \"Controls for the conformance pack. A control is a process to prevent or detect problems while meeting objectives. A control can align with a specific compliance regime or map to internal controls defined by an organization.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-rule-compliance-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: ConformancePackRuleCompliance
---
