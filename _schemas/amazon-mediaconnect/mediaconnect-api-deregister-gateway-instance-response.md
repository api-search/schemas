---
description: DeregisterGatewayInstanceResponse schema from AWS Elemental MediaConnect API
layout: schema
name: DeregisterGatewayInstanceResponse
properties_list:
- description: ''
  name: GatewayInstanceArn
  type: object
- description: ''
  name: InstanceState
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-deregister-gateway-instance-response-schema.json
slug: mediaconnect-api-deregister-gateway-instance-response
source_filename: mediaconnect-api-deregister-gateway-instance-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-deregister-gateway-instance-response-schema.json\",\n  \"title\": \"DeregisterGatewayInstanceResponse\",\n  \"description\": \"DeregisterGatewayInstanceResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayInstanceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gatewayInstanceArn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) of the instance.\"\n        }\n      ]\n    },\n    \"InstanceState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"instanceState\"\n    \
  \      },\n          \"description\": \"The status of the instance.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-deregister-gateway-instance-response-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: DeregisterGatewayInstanceResponse
---
