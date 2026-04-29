---
description: ListMobileDeviceAccessRulesResponse schema from Amazon WorkMail API
layout: schema
name: ListMobileDeviceAccessRulesResponse
properties_list:
- description: ''
  name: Rules
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-list-mobile-device-access-rules-response-schema.json
slug: workmail-list-mobile-device-access-rules-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Rules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MobileDeviceAccessRulesList\"\n        },\n        {\n          \"description\": \"The list of mobile device access rules that exist under the specified WorkMail organization.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListMobileDeviceAccessRulesResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-mobile-device-access-rules-response-schema.json\",\n  \"description\": \"ListMobileDeviceAccessRulesResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-mobile-device-access-rules-response-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ListMobileDeviceAccessRulesResponse
---
