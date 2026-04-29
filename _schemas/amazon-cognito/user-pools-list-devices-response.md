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
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-list-devices-response-schema.json
slug: user-pools-list-devices-response
source_filename: user-pools-list-devices-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-devices-response-schema.json\",\n  \"title\": \"ListDevicesResponse\",\n  \"description\": \"Represents the response to list devices.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Devices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceListType\"\n        },\n        {\n          \"description\": \"The devices returned in the list devices response.\"\n        }\n      ]\n    },\n    \"PaginationToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SearchPaginationTokenType\"\n        },\n        {\n          \"description\": \"The pagination token for the list device response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-devices-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: ListDevicesResponse
---
