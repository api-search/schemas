---
description: GetMobileDeviceAccessEffectRequest schema from Amazon WorkMail API
layout: schema
name: GetMobileDeviceAccessEffectRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: DeviceType
  type: object
- description: ''
  name: DeviceModel
  type: object
- description: ''
  name: DeviceOperatingSystem
  type: object
- description: ''
  name: DeviceUserAgent
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-get-mobile-device-access-effect-request-schema.json
slug: workmail-get-mobile-device-access-effect-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\"\n  ],\n  \"title\": \"GetMobileDeviceAccessEffectRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The WorkMail organization to simulate the access effect for.\"\n        }\n      ]\n    },\n    \"DeviceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceType\"\n        },\n        {\n          \"description\": \"Device type the simulated user will report.\"\n        }\n      ]\n    },\n    \"DeviceModel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceModel\"\n        },\n        {\n          \"description\": \"Device model the simulated user will report.\"\n        }\n      ]\n    },\n    \"DeviceOperatingSystem\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceOperatingSystem\"\
  \n        },\n        {\n          \"description\": \"Device operating system the simulated user will report.\"\n        }\n      ]\n    },\n    \"DeviceUserAgent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceUserAgent\"\n        },\n        {\n          \"description\": \"Device user agent the simulated user will report.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-get-mobile-device-access-effect-request-schema.json\",\n  \"description\": \"GetMobileDeviceAccessEffectRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-get-mobile-device-access-effect-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: GetMobileDeviceAccessEffectRequest
---
