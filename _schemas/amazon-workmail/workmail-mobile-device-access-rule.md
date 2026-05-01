---
description: A rule that controls access to mobile devices for an WorkMail group.
layout: schema
name: MobileDeviceAccessRule
properties_list:
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
- description: ''
  name: DateCreated
  type: object
- description: ''
  name: DateModified
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-mobile-device-access-rule-schema.json
slug: workmail-mobile-device-access-rule
source_filename: workmail-mobile-device-access-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"MobileDeviceAccessRuleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MobileDeviceAccessRuleId\"\n        },\n        {\n          \"description\": \"The ID assigned to a mobile access rule.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MobileDeviceAccessRuleName\"\n        },\n        {\n          \"description\": \"The name of a mobile access rule.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MobileDeviceAccessRuleDescription\"\n        },\n        {\n          \"description\": \"The description of a mobile access rule.\"\n        }\n      ]\n    },\n    \"Effect\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MobileDeviceAccessRuleEffect\"\n        },\n        {\n          \"description\": \"The\
  \ effect of the rule when it matches. Allowed values are <code>ALLOW</code> or <code>DENY</code>.\"\n        }\n      ]\n    },\n    \"DeviceTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceTypeList\"\n        },\n        {\n          \"description\": \"Device types that a rule will match.\"\n        }\n      ]\n    },\n    \"NotDeviceTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceTypeList\"\n        },\n        {\n          \"description\": \"Device types that a rule <b>will not</b> match. All other device types will match.\"\n        }\n      ]\n    },\n    \"DeviceModels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceModelList\"\n        },\n        {\n          \"description\": \"Device models that a rule will match.\"\n        }\n      ]\n    },\n    \"NotDeviceModels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceModelList\"\
  \n        },\n        {\n          \"description\": \"Device models that a rule <b>will not</b> match. All other device models will match.\"\n        }\n      ]\n    },\n    \"DeviceOperatingSystems\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceOperatingSystemList\"\n        },\n        {\n          \"description\": \"Device operating systems that a rule will match.\"\n        }\n      ]\n    },\n    \"NotDeviceOperatingSystems\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceOperatingSystemList\"\n        },\n        {\n          \"description\": \"Device operating systems that a rule <b>will not</b> match. All other device types will match.\"\n        }\n      ]\n    },\n    \"DeviceUserAgents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceUserAgentList\"\n        },\n        {\n          \"description\": \"Device user agents that a rule will match.\"\n        }\n     \
  \ ]\n    },\n    \"NotDeviceUserAgents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceUserAgentList\"\n        },\n        {\n          \"description\": \"Device user agents that a rule <b>will not</b> match. All other device user agents will match.\"\n        }\n      ]\n    },\n    \"DateCreated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time at which an access rule was created.\"\n        }\n      ]\n    },\n    \"DateModified\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time at which an access rule was modified.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A rule that controls access to mobile devices for an WorkMail group.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"\
  MobileDeviceAccessRule\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-mobile-device-access-rule-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-mobile-device-access-rule-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: MobileDeviceAccessRule
---
