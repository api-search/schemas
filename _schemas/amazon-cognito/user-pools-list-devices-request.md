---
description: Represents the request to list the devices.
layout: schema
name: ListDevicesRequest
properties_list:
- description: ''
  name: AccessToken
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: PaginationToken
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-list-devices-request-schema.json
slug: user-pools-list-devices-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-devices-request-schema.json\",\n  \"title\": \"ListDevicesRequest\",\n  \"description\": \"Represents the request to list the devices.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\": \"A valid access token that Amazon Cognito issued to the user whose list of devices you want to view.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryLimitType\"\n        },\n        {\n          \"description\": \"The limit of the device request.\"\n        }\n      ]\n    },\n    \"PaginationToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SearchPaginationTokenType\"\
  \n        },\n        {\n          \"description\": \"The pagination token for the list request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccessToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-devices-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: ListDevicesRequest
---
