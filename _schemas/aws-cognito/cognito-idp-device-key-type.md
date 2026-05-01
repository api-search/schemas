---
description: DeviceKeyType schema from Amazon Cognito
layout: schema
name: DeviceKeyType
properties_list: []
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-device-key-type-schema.json
slug: cognito-idp-device-key-type
source_filename: cognito-idp-device-key-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"string\",\n  \"pattern\": \"[\\\\w-]+_[0-9a-f-]+\",\n  \"minLength\": 1,\n  \"maxLength\": 55,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-device-key-type-schema.json\",\n  \"title\": \"DeviceKeyType\",\n  \"description\": \"DeviceKeyType schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-device-key-type-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: DeviceKeyType
---
