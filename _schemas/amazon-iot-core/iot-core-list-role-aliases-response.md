---
description: ListRoleAliasesResponse schema
layout: schema
name: ListRoleAliasesResponse
properties_list:
- description: ''
  name: roleAliases
  type: object
- description: ''
  name: nextMarker
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-list-role-aliases-response-schema.json
slug: iot-core-list-role-aliases-response
source_filename: iot-core-list-role-aliases-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-role-aliases-response-schema.json\",\n  \"title\": \"ListRoleAliasesResponse\",\n  \"description\": \"ListRoleAliasesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"roleAliases\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleAliases\"\n        },\n        {\n          \"description\": \"The role aliases.\"\n        }\n      ]\n    },\n    \"nextMarker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"A marker used to get the next set of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-role-aliases-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: ListRoleAliasesResponse
---
