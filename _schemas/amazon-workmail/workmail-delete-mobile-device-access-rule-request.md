---
description: DeleteMobileDeviceAccessRuleRequest schema from Amazon WorkMail API
layout: schema
name: DeleteMobileDeviceAccessRuleRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: MobileDeviceAccessRuleId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-delete-mobile-device-access-rule-request-schema.json
slug: workmail-delete-mobile-device-access-rule-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"MobileDeviceAccessRuleId\"\n  ],\n  \"title\": \"DeleteMobileDeviceAccessRuleRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The WorkMail organization under which the rule will be deleted.\"\n        }\n      ]\n    },\n    \"MobileDeviceAccessRuleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MobileDeviceAccessRuleId\"\n        },\n        {\n          \"description\": \"The identifier of the rule to be deleted.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delete-mobile-device-access-rule-request-schema.json\",\n  \"description\": \"DeleteMobileDeviceAccessRuleRequest\
  \ schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delete-mobile-device-access-rule-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DeleteMobileDeviceAccessRuleRequest
---
