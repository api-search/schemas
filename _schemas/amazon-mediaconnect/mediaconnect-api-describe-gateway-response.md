---
description: DescribeGatewayResponse schema from AWS Elemental MediaConnect API
layout: schema
name: DescribeGatewayResponse
properties_list:
- description: ''
  name: Gateway
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-describe-gateway-response-schema.json
slug: mediaconnect-api-describe-gateway-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-describe-gateway-response-schema.json\",\n  \"title\": \"DescribeGatewayResponse\",\n  \"description\": \"DescribeGatewayResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Gateway\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Gateway\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gateway\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-describe-gateway-response-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: DescribeGatewayResponse
---
