---
description: The rule that a simulated user matches.
layout: schema
name: MobileDeviceAccessMatchedRule
properties_list:
- description: ''
  name: MobileDeviceAccessRuleId
  type: object
- description: ''
  name: Name
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-mobile-device-access-matched-rule-schema.json
slug: workmail-mobile-device-access-matched-rule
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"MobileDeviceAccessRuleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MobileDeviceAccessRuleId\"\n        },\n        {\n          \"description\": \"Identifier of the rule that a simulated user matches.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MobileDeviceAccessRuleName\"\n        },\n        {\n          \"description\": \"Name of a rule that a simulated user matches.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The rule that a simulated user matches.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MobileDeviceAccessMatchedRule\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-mobile-device-access-matched-rule-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-mobile-device-access-matched-rule-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: MobileDeviceAccessMatchedRule
---
