---
description: DescribeDefaultAuthorizerResponse schema
layout: schema
name: DescribeDefaultAuthorizerResponse
properties_list:
- description: ''
  name: authorizerDescription
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-describe-default-authorizer-response-schema.json
slug: iot-device-defender-describe-default-authorizer-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-default-authorizer-response-schema.json\",\n  \"title\": \"DescribeDefaultAuthorizerResponse\",\n  \"description\": \"DescribeDefaultAuthorizerResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authorizerDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthorizerDescription\"\n        },\n        {\n          \"description\": \"The default authorizer's description.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-default-authorizer-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: DescribeDefaultAuthorizerResponse
---
