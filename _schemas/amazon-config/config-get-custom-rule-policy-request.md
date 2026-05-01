---
description: GetCustomRulePolicyRequest schema
layout: schema
name: GetCustomRulePolicyRequest
properties_list:
- description: ''
  name: ConfigRuleName
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-custom-rule-policy-request-schema.json
slug: config-get-custom-rule-policy-request
source_filename: config-get-custom-rule-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-custom-rule-policy-request-schema.json\",\n  \"title\": \"GetCustomRulePolicyRequest\",\n  \"description\": \"GetCustomRulePolicyRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRuleName\"\n        },\n        {\n          \"description\": \"The name of your Config Custom Policy rule.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-custom-rule-policy-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: GetCustomRulePolicyRequest
---
