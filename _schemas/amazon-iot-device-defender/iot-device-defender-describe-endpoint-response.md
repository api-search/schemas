---
description: The output from the DescribeEndpoint operation.
layout: schema
name: DescribeEndpointResponse
properties_list:
- description: ''
  name: endpointAddress
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-describe-endpoint-response-schema.json
slug: iot-device-defender-describe-endpoint-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-endpoint-response-schema.json\",\n  \"title\": \"DescribeEndpointResponse\",\n  \"description\": \"The output from the DescribeEndpoint operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endpointAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointAddress\"\n        },\n        {\n          \"description\": \"The endpoint. The format of the endpoint is as follows: <i>identifier</i>.iot.<i>region</i>.amazonaws.com.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-endpoint-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: DescribeEndpointResponse
---
