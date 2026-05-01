---
description: The impersonation rule that matched the input.
layout: schema
name: ImpersonationMatchedRule
properties_list:
- description: ''
  name: ImpersonationRuleId
  type: object
- description: ''
  name: Name
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-impersonation-matched-rule-schema.json
slug: workmail-impersonation-matched-rule
source_filename: workmail-impersonation-matched-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ImpersonationRuleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRuleId\"\n        },\n        {\n          \"description\": \"The ID of the rule that matched the input\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRuleName\"\n        },\n        {\n          \"description\": \"The name of the rule that matched the input.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The impersonation rule that matched the input.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ImpersonationMatchedRule\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-impersonation-matched-rule-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-impersonation-matched-rule-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ImpersonationMatchedRule
---
