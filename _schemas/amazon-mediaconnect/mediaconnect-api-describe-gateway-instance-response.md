---
description: DescribeGatewayInstanceResponse schema from AWS Elemental MediaConnect API
layout: schema
name: DescribeGatewayInstanceResponse
properties_list:
- description: ''
  name: GatewayInstance
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-describe-gateway-instance-response-schema.json
slug: mediaconnect-api-describe-gateway-instance-response
source_filename: mediaconnect-api-describe-gateway-instance-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-describe-gateway-instance-response-schema.json\",\n  \"title\": \"DescribeGatewayInstanceResponse\",\n  \"description\": \"DescribeGatewayInstanceResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayInstance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayInstance\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gatewayInstance\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-describe-gateway-instance-response-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: DescribeGatewayInstanceResponse
---
