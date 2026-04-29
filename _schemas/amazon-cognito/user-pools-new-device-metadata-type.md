---
description: The new device metadata type.
layout: schema
name: NewDeviceMetadataType
properties_list:
- description: ''
  name: DeviceKey
  type: object
- description: ''
  name: DeviceGroupKey
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-new-device-metadata-type-schema.json
slug: user-pools-new-device-metadata-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-new-device-metadata-type-schema.json\",\n  \"title\": \"NewDeviceMetadataType\",\n  \"description\": \"The new device metadata type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeviceKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceKeyType\"\n        },\n        {\n          \"description\": \"The device key.\"\n        }\n      ]\n    },\n    \"DeviceGroupKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The device group key.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-new-device-metadata-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: NewDeviceMetadataType
---
