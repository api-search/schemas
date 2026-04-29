---
description: Gets the device response, as an administrator.
layout: schema
name: AdminGetDeviceResponse
properties_list:
- description: ''
  name: Device
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-admin-get-device-response-schema.json
slug: cognito-idp-admin-get-device-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Device\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceType\"\n        },\n        {\n          \"description\": \"The device.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Device\"\n  ],\n  \"description\": \"Gets the device response, as an administrator.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-get-device-response-schema.json\",\n  \"title\": \"AdminGetDeviceResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-get-device-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: AdminGetDeviceResponse
---
