---
description: Confirms the device response.
layout: schema
name: ConfirmDeviceResponse
properties_list:
- description: ''
  name: UserConfirmationNecessary
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-confirm-device-response-schema.json
slug: user-pools-confirm-device-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-confirm-device-response-schema.json\",\n  \"title\": \"ConfirmDeviceResponse\",\n  \"description\": \"Confirms the device response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserConfirmationNecessary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanType\"\n        },\n        {\n          \"description\": \"Indicates whether the user confirmation must confirm the device response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-confirm-device-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: ConfirmDeviceResponse
---
