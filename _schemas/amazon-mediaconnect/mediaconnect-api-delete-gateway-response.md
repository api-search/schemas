---
description: DeleteGatewayResponse schema from AWS Elemental MediaConnect API
layout: schema
name: DeleteGatewayResponse
properties_list:
- description: ''
  name: GatewayArn
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-delete-gateway-response-schema.json
slug: mediaconnect-api-delete-gateway-response
source_filename: mediaconnect-api-delete-gateway-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-delete-gateway-response-schema.json\",\n  \"title\": \"DeleteGatewayResponse\",\n  \"description\": \"DeleteGatewayResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gatewayArn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) of the gateway that was deleted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-delete-gateway-response-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: DeleteGatewayResponse
---
