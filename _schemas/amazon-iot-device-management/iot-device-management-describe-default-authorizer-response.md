---
description: DescribeDefaultAuthorizerResponse schema
layout: schema
name: DescribeDefaultAuthorizerResponse
properties_list:
- description: ''
  name: authorizerDescription
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-describe-default-authorizer-response-schema.json
slug: iot-device-management-describe-default-authorizer-response
source_filename: iot-device-management-describe-default-authorizer-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-default-authorizer-response-schema.json\",\n  \"title\": \"DescribeDefaultAuthorizerResponse\",\n  \"description\": \"DescribeDefaultAuthorizerResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authorizerDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthorizerDescription\"\n        },\n        {\n          \"description\": \"The default authorizer's description.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-default-authorizer-response-schema.json
tags:
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: DescribeDefaultAuthorizerResponse
---
