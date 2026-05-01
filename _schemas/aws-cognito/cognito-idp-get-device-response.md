---
description: Gets the device response.
layout: schema
name: GetDeviceResponse
properties_list:
- description: ''
  name: Device
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-get-device-response-schema.json
slug: cognito-idp-get-device-response
source_filename: cognito-idp-get-device-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Device\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceType\"\n        },\n        {\n          \"description\": \"The device.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Device\"\n  ],\n  \"description\": \"Gets the device response.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-get-device-response-schema.json\",\n  \"title\": \"GetDeviceResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-get-device-response-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: GetDeviceResponse
---
