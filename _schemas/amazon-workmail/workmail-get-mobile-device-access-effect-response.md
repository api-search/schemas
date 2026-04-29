---
description: GetMobileDeviceAccessEffectResponse schema from Amazon WorkMail API
layout: schema
name: GetMobileDeviceAccessEffectResponse
properties_list:
- description: ''
  name: Effect
  type: object
- description: ''
  name: MatchedRules
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-get-mobile-device-access-effect-response-schema.json
slug: workmail-get-mobile-device-access-effect-response
source_filename: workmail-get-mobile-device-access-effect-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Effect\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MobileDeviceAccessRuleEffect\"\n        },\n        {\n          \"description\": \"The effect of the simulated access, <code>ALLOW</code> or <code>DENY</code>, after evaluating mobile device access rules in the WorkMail organization for the simulated user parameters.\"\n        }\n      ]\n    },\n    \"MatchedRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MobileDeviceAccessMatchedRuleList\"\n        },\n        {\n          \"description\": \"A list of the rules which matched the simulated user input and produced the effect.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetMobileDeviceAccessEffectResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-get-mobile-device-access-effect-response-schema.json\"\
  ,\n  \"description\": \"GetMobileDeviceAccessEffectResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-get-mobile-device-access-effect-response-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: GetMobileDeviceAccessEffectResponse
---
