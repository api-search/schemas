---
description: DescribeRoleAliasResponse schema
layout: schema
name: DescribeRoleAliasResponse
properties_list:
- description: ''
  name: roleAliasDescription
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-describe-role-alias-response-schema.json
slug: iot-device-management-describe-role-alias-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-role-alias-response-schema.json\",\n  \"title\": \"DescribeRoleAliasResponse\",\n  \"description\": \"DescribeRoleAliasResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"roleAliasDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleAliasDescription\"\n        },\n        {\n          \"description\": \"The role alias description.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-role-alias-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: DescribeRoleAliasResponse
---
