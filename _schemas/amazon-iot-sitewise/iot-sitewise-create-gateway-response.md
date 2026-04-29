---
description: CreateGatewayResponse schema
layout: schema
name: CreateGatewayResponse
properties_list:
- description: ''
  name: gatewayId
  type: object
- description: ''
  name: gatewayArn
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-create-gateway-response-schema.json
slug: iot-sitewise-create-gateway-response
source_filename: iot-sitewise-create-gateway-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-create-gateway-response-schema.json\",\n  \"title\": \"CreateGatewayResponse\",\n  \"description\": \"CreateGatewayResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"gatewayId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the gateway device. You can use this ID when you call other IoT SiteWise APIs.\"\n        }\n      ]\n    },\n    \"gatewayArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"<p>The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the gateway, which has the following format.</p> <p> <code>arn:${Partition}:iotsitewise:${Region}:${Account}:gateway/${GatewayId}</code>\
  \ </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"gatewayId\",\n    \"gatewayArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-create-gateway-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: CreateGatewayResponse
---
