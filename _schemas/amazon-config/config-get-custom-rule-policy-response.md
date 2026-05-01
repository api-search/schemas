---
description: GetCustomRulePolicyResponse schema
layout: schema
name: GetCustomRulePolicyResponse
properties_list:
- description: ''
  name: PolicyText
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-custom-rule-policy-response-schema.json
slug: config-get-custom-rule-policy-response
source_filename: config-get-custom-rule-policy-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-custom-rule-policy-response-schema.json\",\n  \"title\": \"GetCustomRulePolicyResponse\",\n  \"description\": \"GetCustomRulePolicyResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PolicyText\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyText\"\n        },\n        {\n          \"description\": \"The policy definition containing the logic for your Config Custom Policy rule.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-custom-rule-policy-response-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: GetCustomRulePolicyResponse
---
