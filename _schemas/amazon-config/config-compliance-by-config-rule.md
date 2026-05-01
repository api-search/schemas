---
description: Indicates whether an Config rule is compliant. A rule is compliant if all of the resources that the rule evaluated comply with it. A rule is noncompliant if any of these resources do not comply.
layout: schema
name: ComplianceByConfigRule
properties_list:
- description: ''
  name: ConfigRuleName
  type: object
- description: ''
  name: Compliance
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-compliance-by-config-rule-schema.json
slug: config-compliance-by-config-rule
source_filename: config-compliance-by-config-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-compliance-by-config-rule-schema.json\",\n  \"title\": \"ComplianceByConfigRule\",\n  \"description\": \"Indicates whether an Config rule is compliant. A rule is compliant if all of the resources that the rule evaluated comply with it. A rule is noncompliant if any of these resources do not comply.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit64\"\n        },\n        {\n          \"description\": \"The name of the Config rule.\"\n        }\n      ]\n    },\n    \"Compliance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Compliance\"\n        },\n        {\n          \"description\": \"Indicates whether the Config rule is compliant.\"\n     \
  \   }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-compliance-by-config-rule-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: ComplianceByConfigRule
---
