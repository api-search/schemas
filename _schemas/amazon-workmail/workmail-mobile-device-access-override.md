---
description: The override object.
layout: schema
name: MobileDeviceAccessOverride
properties_list:
- description: ''
  name: UserId
  type: object
- description: ''
  name: DeviceId
  type: object
- description: ''
  name: Effect
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: DateCreated
  type: object
- description: ''
  name: DateModified
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-mobile-device-access-override-schema.json
slug: workmail-mobile-device-access-override
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The WorkMail user to which the access override applies.\"\n        }\n      ]\n    },\n    \"DeviceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceId\"\n        },\n        {\n          \"description\": \"The device to which the override applies.\"\n        }\n      ]\n    },\n    \"Effect\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MobileDeviceAccessRuleEffect\"\n        },\n        {\n          \"description\": \"The effect of the override, <code>ALLOW</code> or <code>DENY</code>.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MobileDeviceAccessRuleDescription\"\n        },\n        {\n          \"description\"\
  : \"A description of the override.\"\n        }\n      ]\n    },\n    \"DateCreated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the override was first created.\"\n        }\n      ]\n    },\n    \"DateModified\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the override was last modified.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The override object.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MobileDeviceAccessOverride\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-mobile-device-access-override-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-mobile-device-access-override-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: MobileDeviceAccessOverride
---
