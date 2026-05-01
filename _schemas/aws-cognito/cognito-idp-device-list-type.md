---
description: DeviceListType schema from Amazon Cognito
layout: schema
name: DeviceListType
properties_list: []
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-device-list-type-schema.json
slug: cognito-idp-device-list-type
source_filename: cognito-idp-device-list-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"DeviceKey\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DeviceKeyType\"\n          },\n          {\n            \"description\": \"The device key.\"\n          }\n        ]\n      },\n      \"DeviceAttributes\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AttributeListType\"\n          },\n          {\n            \"description\": \"The device attributes.\"\n          }\n        ]\n      },\n      \"DeviceCreateDate\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DateType\"\n          },\n          {\n            \"description\": \"The creation date of the device.\"\n          }\n        ]\n      },\n      \"DeviceLastModifiedDate\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DateType\"\n          },\n          {\n     \
  \       \"description\": \"The last modified date of the device.\"\n          }\n        ]\n      },\n      \"DeviceLastAuthenticatedDate\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DateType\"\n          },\n          {\n            \"description\": \"The date when the device was last authenticated.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"The device type.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-device-list-type-schema.json\",\n  \"title\": \"DeviceListType\",\n  \"description\": \"DeviceListType schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-device-list-type-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: DeviceListType
---
