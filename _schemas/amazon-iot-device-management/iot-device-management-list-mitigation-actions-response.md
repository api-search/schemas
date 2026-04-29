---
description: ListMitigationActionsResponse schema
layout: schema
name: ListMitigationActionsResponse
properties_list:
- description: ''
  name: actionIdentifiers
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-list-mitigation-actions-response-schema.json
slug: iot-device-management-list-mitigation-actions-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-mitigation-actions-response-schema.json\",\n  \"title\": \"ListMitigationActionsResponse\",\n  \"description\": \"ListMitigationActionsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionIdentifiers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MitigationActionIdentifierList\"\n        },\n        {\n          \"description\": \"A set of actions that matched the specified filter criteria.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for the next set of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-mitigation-actions-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: ListMitigationActionsResponse
---
