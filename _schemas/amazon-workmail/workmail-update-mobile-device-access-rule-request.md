---
description: UpdateMobileDeviceAccessRuleRequest schema from Amazon WorkMail API
layout: schema
name: UpdateMobileDeviceAccessRuleRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: MobileDeviceAccessRuleId
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
  name: DeviceTypes
  type: object
- description: ''
  name: NotDeviceTypes
  type: object
- description: ''
  name: DeviceModels
  type: object
- description: ''
  name: NotDeviceModels
  type: object
- description: ''
  name: DeviceOperatingSystems
  type: object
- description: ''
  name: NotDeviceOperatingSystems
  type: object
- description: ''
  name: DeviceUserAgents
  type: object
- description: ''
  name: NotDeviceUserAgents
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-update-mobile-device-access-rule-request-schema.json
slug: workmail-update-mobile-device-access-rule-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"MobileDeviceAccessRuleId\",\n    \"Name\",\n    \"Effect\"\n  ],\n  \"title\": \"UpdateMobileDeviceAccessRuleRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The WorkMail organization under which the rule will be updated.\"\n        }\n      ]\n    },\n    \"MobileDeviceAccessRuleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MobileDeviceAccessRuleId\"\n        },\n        {\n          \"description\": \"The identifier of the rule to be updated.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MobileDeviceAccessRuleName\"\n        },\n        {\n          \"description\": \"The updated rule name.\"\n        }\n      ]\n    },\n    \"Description\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MobileDeviceAccessRuleDescription\"\n        },\n        {\n          \"description\": \"The updated rule description.\"\n        }\n      ]\n    },\n    \"Effect\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MobileDeviceAccessRuleEffect\"\n        },\n        {\n          \"description\": \"The effect of the rule when it matches. Allowed values are <code>ALLOW</code> or <code>DENY</code>.\"\n        }\n      ]\n    },\n    \"DeviceTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceTypeList\"\n        },\n        {\n          \"description\": \"Device types that the updated rule will match.\"\n        }\n      ]\n    },\n    \"NotDeviceTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceTypeList\"\n        },\n        {\n          \"description\": \"Device types that the updated rule <b>will not</b>\
  \ match. All other device types will match.\"\n        }\n      ]\n    },\n    \"DeviceModels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceModelList\"\n        },\n        {\n          \"description\": \"Device models that the updated rule will match.\"\n        }\n      ]\n    },\n    \"NotDeviceModels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceModelList\"\n        },\n        {\n          \"description\": \"Device models that the updated rule <b>will not</b> match. All other device models will match.\"\n        }\n      ]\n    },\n    \"DeviceOperatingSystems\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceOperatingSystemList\"\n        },\n        {\n          \"description\": \"Device operating systems that the updated rule will match.\"\n        }\n      ]\n    },\n    \"NotDeviceOperatingSystems\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceOperatingSystemList\"\
  \n        },\n        {\n          \"description\": \"Device operating systems that the updated rule <b>will not</b> match. All other device operating systems will match.\"\n        }\n      ]\n    },\n    \"DeviceUserAgents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceUserAgentList\"\n        },\n        {\n          \"description\": \"User agents that the updated rule will match.\"\n        }\n      ]\n    },\n    \"NotDeviceUserAgents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceUserAgentList\"\n        },\n        {\n          \"description\": \"User agents that the updated rule <b>will not</b> match. All other user agents will match.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-update-mobile-device-access-rule-request-schema.json\"\
  ,\n  \"description\": \"UpdateMobileDeviceAccessRuleRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-update-mobile-device-access-rule-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: UpdateMobileDeviceAccessRuleRequest
---
