---
description: The device verifier against which it is authenticated.
layout: schema
name: DeviceSecretVerifierConfigType
properties_list:
- description: ''
  name: PasswordVerifier
  type: object
- description: ''
  name: Salt
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-device-secret-verifier-config-type-schema.json
slug: cognito-idp-device-secret-verifier-config-type
source_filename: cognito-idp-device-secret-verifier-config-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"PasswordVerifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The password verifier.\"\n        }\n      ]\n    },\n    \"Salt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://en.wikipedia.org/wiki/Salt_(cryptography)\\\">salt</a> \"\n        }\n      ]\n    }\n  },\n  \"description\": \"The device verifier against which it is authenticated.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-device-secret-verifier-config-type-schema.json\",\n  \"title\": \"DeviceSecretVerifierConfigType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-device-secret-verifier-config-type-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: DeviceSecretVerifierConfigType
---
