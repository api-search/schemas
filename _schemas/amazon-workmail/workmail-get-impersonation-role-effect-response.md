---
description: GetImpersonationRoleEffectResponse schema from Amazon WorkMail API
layout: schema
name: GetImpersonationRoleEffectResponse
properties_list:
- description: ''
  name: Type
  type: object
- description: ''
  name: Effect
  type: object
- description: ''
  name: MatchedRules
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-get-impersonation-role-effect-response-schema.json
slug: workmail-get-impersonation-role-effect-response
source_filename: workmail-get-impersonation-role-effect-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRoleType\"\n        },\n        {\n          \"description\": \"The impersonation role type.\"\n        }\n      ]\n    },\n    \"Effect\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessEffect\"\n        },\n        {\n          \"description\": \" <code/>Effect of the impersonation role on the target user based on its rules. Available effects are <code>ALLOW</code> or <code>DENY</code>.\"\n        }\n      ]\n    },\n    \"MatchedRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationMatchedRuleList\"\n        },\n        {\n          \"description\": \"A list of the rules that match the input and produce the configured effect.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"\
  GetImpersonationRoleEffectResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-get-impersonation-role-effect-response-schema.json\",\n  \"description\": \"GetImpersonationRoleEffectResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-get-impersonation-role-effect-response-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: GetImpersonationRoleEffectResponse
---
