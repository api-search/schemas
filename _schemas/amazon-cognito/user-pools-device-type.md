---
description: The device type.
layout: schema
name: DeviceType
properties_list:
- description: ''
  name: DeviceKey
  type: object
- description: ''
  name: DeviceAttributes
  type: object
- description: ''
  name: DeviceCreateDate
  type: object
- description: ''
  name: DeviceLastModifiedDate
  type: object
- description: ''
  name: DeviceLastAuthenticatedDate
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-device-type-schema.json
slug: user-pools-device-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-device-type-schema.json\",\n  \"title\": \"DeviceType\",\n  \"description\": \"The device type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeviceKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceKeyType\"\n        },\n        {\n          \"description\": \"The device key.\"\n        }\n      ]\n    },\n    \"DeviceAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeListType\"\n        },\n        {\n          \"description\": \"The device attributes.\"\n        }\n      ]\n    },\n    \"DeviceCreateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The creation date of the device.\"\n        }\n\
  \      ]\n    },\n    \"DeviceLastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date and time, in <a href=\\\"https://www.iso.org/iso-8601-date-and-time-format.html\\\">ISO 8601</a> format, when the item was modified.\"\n        }\n      ]\n    },\n    \"DeviceLastAuthenticatedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date when the device was last authenticated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-device-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: DeviceType
---
