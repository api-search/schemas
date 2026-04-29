---
description: PutOrganizationConfigRuleResponse schema
layout: schema
name: PutOrganizationConfigRuleResponse
properties_list:
- description: ''
  name: OrganizationConfigRuleArn
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-organization-config-rule-response-schema.json
slug: config-put-organization-config-rule-response
source_filename: config-put-organization-config-rule-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-organization-config-rule-response-schema.json\",\n  \"title\": \"PutOrganizationConfigRuleResponse\",\n  \"description\": \"PutOrganizationConfigRuleResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OrganizationConfigRuleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of an organization Config rule.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-organization-config-rule-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: PutOrganizationConfigRuleResponse
---
