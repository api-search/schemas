---
description: Represents the response to list devices.
layout: schema
name: ListDevicesResponse
properties_list:
- description: ''
  name: Devices
  type: object
- description: ''
  name: PaginationToken
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-list-devices-response-schema.json
slug: cognito-idp-list-devices-response
source_filename: cognito-idp-list-devices-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Devices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceListType\"\n        },\n        {\n          \"description\": \"The devices returned in the list devices response.\"\n        }\n      ]\n    },\n    \"PaginationToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SearchPaginationTokenType\"\n        },\n        {\n          \"description\": \"The pagination token for the list device response.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Represents the response to list devices.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-list-devices-response-schema.json\",\n  \"title\": \"ListDevicesResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-list-devices-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ListDevicesResponse
---
