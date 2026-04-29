---
description: PutConfigRuleRequest schema
layout: schema
name: PutConfigRuleRequest
properties_list:
- description: ''
  name: ConfigRule
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-config-rule-request-schema.json
slug: config-put-config-rule-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-config-rule-request-schema.json\",\n  \"title\": \"PutConfigRuleRequest\",\n  \"description\": \"PutConfigRuleRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRule\"\n        },\n        {\n          \"description\": \"The rule that you want to add to your account.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsList\"\n        },\n        {\n          \"description\": \"An array of tag object.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigRule\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-config-rule-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: PutConfigRuleRequest
---
