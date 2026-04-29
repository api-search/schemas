---
description: DescribeAuthorizerResponse schema
layout: schema
name: DescribeAuthorizerResponse
properties_list:
- description: ''
  name: authorizerDescription
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-describe-authorizer-response-schema.json
slug: iot-device-management-describe-authorizer-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-authorizer-response-schema.json\",\n  \"title\": \"DescribeAuthorizerResponse\",\n  \"description\": \"DescribeAuthorizerResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authorizerDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthorizerDescription\"\n        },\n        {\n          \"description\": \"The authorizer description.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-authorizer-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: DescribeAuthorizerResponse
---
