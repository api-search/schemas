---
description: Provides a summary of a gateway, including its name, ARN, and status.
layout: schema
name: ListedGateway
properties_list:
- description: ''
  name: GatewayArn
  type: object
- description: ''
  name: GatewayState
  type: object
- description: ''
  name: Name
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-listed-gateway-schema.json
slug: mediaconnect-api-listed-gateway
source_filename: mediaconnect-api-listed-gateway-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-listed-gateway-schema.json\",\n  \"title\": \"ListedGateway\",\n  \"description\": \"Provides a summary of a gateway, including its name, ARN, and status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gatewayArn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) of the gateway.\"\n        }\n      ]\n    },\n    \"GatewayState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gatewayState\"\n          }\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the gateway.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GatewayArn\",\n    \"GatewayState\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-listed-gateway-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: ListedGateway
---
