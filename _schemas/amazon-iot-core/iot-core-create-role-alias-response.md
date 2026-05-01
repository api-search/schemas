---
description: CreateRoleAliasResponse schema
layout: schema
name: CreateRoleAliasResponse
properties_list:
- description: ''
  name: roleAlias
  type: object
- description: ''
  name: roleAliasArn
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-create-role-alias-response-schema.json
slug: iot-core-create-role-alias-response
source_filename: iot-core-create-role-alias-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-create-role-alias-response-schema.json\",\n  \"title\": \"CreateRoleAliasResponse\",\n  \"description\": \"CreateRoleAliasResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"roleAlias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleAlias\"\n        },\n        {\n          \"description\": \"The role alias.\"\n        }\n      ]\n    },\n    \"roleAliasArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleAliasArn\"\n        },\n        {\n          \"description\": \"The role alias ARN.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-create-role-alias-response-schema.json
tags:
- Device Management
- IoT
- MQTT
- Message Routing
title: CreateRoleAliasResponse
---
