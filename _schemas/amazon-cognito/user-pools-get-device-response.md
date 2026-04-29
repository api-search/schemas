---
description: Gets the device response.
layout: schema
name: GetDeviceResponse
properties_list:
- description: ''
  name: Device
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-get-device-response-schema.json
slug: user-pools-get-device-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-device-response-schema.json\",\n  \"title\": \"GetDeviceResponse\",\n  \"description\": \"Gets the device response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Device\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceType\"\n        },\n        {\n          \"description\": \"The device.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Device\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-device-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: GetDeviceResponse
---
