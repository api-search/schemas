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
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-list-mitigation-actions-response-schema.json
slug: iot-core-list-mitigation-actions-response
source_filename: iot-core-list-mitigation-actions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-mitigation-actions-response-schema.json\",\n  \"title\": \"ListMitigationActionsResponse\",\n  \"description\": \"ListMitigationActionsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionIdentifiers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MitigationActionIdentifierList\"\n        },\n        {\n          \"description\": \"A set of actions that matched the specified filter criteria.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for the next set of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-mitigation-actions-response-schema.json
tags:
- Device Management
- IoT
- MQTT
- Message Routing
title: ListMitigationActionsResponse
---
