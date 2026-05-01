---
description: Represents the request to get the device, as an administrator.
layout: schema
name: AdminGetDeviceRequest
properties_list:
- description: ''
  name: DeviceKey
  type: object
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: Username
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-admin-get-device-request-schema.json
slug: cognito-idp-admin-get-device-request
source_filename: cognito-idp-admin-get-device-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeviceKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceKeyType\"\n        },\n        {\n          \"description\": \"The device key.\"\n        }\n      ]\n    },\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID.\"\n        }\n      ]\n    },\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsernameType\"\n        },\n        {\n          \"description\": \"The user name.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DeviceKey\",\n    \"UserPoolId\",\n    \"Username\"\n  ],\n  \"description\": \"Represents the request to get the device, as an administrator.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-get-device-request-schema.json\"\
  ,\n  \"title\": \"AdminGetDeviceRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-get-device-request-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: AdminGetDeviceRequest
---
