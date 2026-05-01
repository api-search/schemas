---
description: GetAccessControlEffectResponse schema from Amazon WorkMail API
layout: schema
name: GetAccessControlEffectResponse
properties_list:
- description: ''
  name: Effect
  type: object
- description: ''
  name: MatchedRules
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-get-access-control-effect-response-schema.json
slug: workmail-get-access-control-effect-response
source_filename: workmail-get-access-control-effect-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Effect\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessControlRuleEffect\"\n        },\n        {\n          \"description\": \"The rule effect.\"\n        }\n      ]\n    },\n    \"MatchedRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessControlRuleNameList\"\n        },\n        {\n          \"description\": \"The rules that match the given parameters, resulting in an effect.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetAccessControlEffectResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-get-access-control-effect-response-schema.json\",\n  \"description\": \"GetAccessControlEffectResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-get-access-control-effect-response-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: GetAccessControlEffectResponse
---
