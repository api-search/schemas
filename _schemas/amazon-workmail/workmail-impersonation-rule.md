---
description: The rules for the given impersonation role.
layout: schema
name: ImpersonationRule
properties_list:
- description: ''
  name: ImpersonationRuleId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Effect
  type: object
- description: ''
  name: TargetUsers
  type: object
- description: ''
  name: NotTargetUsers
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-impersonation-rule-schema.json
slug: workmail-impersonation-rule
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ImpersonationRuleId\",\n    \"Effect\"\n  ],\n  \"properties\": {\n    \"ImpersonationRuleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRuleId\"\n        },\n        {\n          \"description\": \"The identifier of the rule.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRuleName\"\n        },\n        {\n          \"description\": \"The rule name.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRuleDescription\"\n        },\n        {\n          \"description\": \"The rule description.\"\n        }\n      ]\n    },\n    \"Effect\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessEffect\"\n        },\n        {\n          \"description\": \"The effect of the\
  \ rule when it matches the input. Allowed effect values are <code>ALLOW</code> or <code>DENY</code>.\"\n        }\n      ]\n    },\n    \"TargetUsers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetUsers\"\n        },\n        {\n          \"description\": \"A list of user IDs that match the rule.\"\n        }\n      ]\n    },\n    \"NotTargetUsers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetUsers\"\n        },\n        {\n          \"description\": \"A list of user IDs that don't match the rule.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The rules for the given impersonation role.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ImpersonationRule\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-impersonation-rule-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-impersonation-rule-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ImpersonationRule
---
