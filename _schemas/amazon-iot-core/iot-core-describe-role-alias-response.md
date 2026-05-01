---
description: DescribeRoleAliasResponse schema
layout: schema
name: DescribeRoleAliasResponse
properties_list:
- description: ''
  name: roleAliasDescription
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-describe-role-alias-response-schema.json
slug: iot-core-describe-role-alias-response
source_filename: iot-core-describe-role-alias-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-describe-role-alias-response-schema.json\",\n  \"title\": \"DescribeRoleAliasResponse\",\n  \"description\": \"DescribeRoleAliasResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"roleAliasDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleAliasDescription\"\n        },\n        {\n          \"description\": \"The role alias description.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-describe-role-alias-response-schema.json
tags:
- Device Management
- IoT
- MQTT
- Message Routing
title: DescribeRoleAliasResponse
---
