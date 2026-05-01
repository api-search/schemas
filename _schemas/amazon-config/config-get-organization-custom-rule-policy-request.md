---
description: GetOrganizationCustomRulePolicyRequest schema
layout: schema
name: GetOrganizationCustomRulePolicyRequest
properties_list:
- description: ''
  name: OrganizationConfigRuleName
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-organization-custom-rule-policy-request-schema.json
slug: config-get-organization-custom-rule-policy-request
source_filename: config-get-organization-custom-rule-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-organization-custom-rule-policy-request-schema.json\",\n  \"title\": \"GetOrganizationCustomRulePolicyRequest\",\n  \"description\": \"GetOrganizationCustomRulePolicyRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OrganizationConfigRuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationConfigRuleName\"\n        },\n        {\n          \"description\": \"The name of your organization Config Custom Policy rule. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"OrganizationConfigRuleName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-organization-custom-rule-policy-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: GetOrganizationCustomRulePolicyRequest
---
