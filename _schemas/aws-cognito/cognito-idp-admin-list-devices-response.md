---
description: Lists the device's response, as an administrator.
layout: schema
name: AdminListDevicesResponse
properties_list:
- description: ''
  name: Devices
  type: object
- description: ''
  name: PaginationToken
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-admin-list-devices-response-schema.json
slug: cognito-idp-admin-list-devices-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Devices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceListType\"\n        },\n        {\n          \"description\": \"The devices in the list of devices response.\"\n        }\n      ]\n    },\n    \"PaginationToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SearchPaginationTokenType\"\n        },\n        {\n          \"description\": \"The pagination token.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Lists the device's response, as an administrator.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-list-devices-response-schema.json\",\n  \"title\": \"AdminListDevicesResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-list-devices-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: AdminListDevicesResponse
---
