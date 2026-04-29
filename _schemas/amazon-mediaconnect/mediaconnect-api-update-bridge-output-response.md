---
description: UpdateBridgeOutputResponse schema from AWS Elemental MediaConnect API
layout: schema
name: UpdateBridgeOutputResponse
properties_list:
- description: ''
  name: BridgeArn
  type: object
- description: ''
  name: Output
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-update-bridge-output-response-schema.json
slug: mediaconnect-api-update-bridge-output-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-bridge-output-response-schema.json\",\n  \"title\": \"UpdateBridgeOutputResponse\",\n  \"description\": \"UpdateBridgeOutputResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BridgeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bridgeArn\"\n          },\n          \"description\": \"The Amazon Resource Number (ARN) of the bridge.\"\n        }\n      ]\n    },\n    \"Output\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BridgeOutput\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"output\"\n          },\n          \"description\": \"The output that\
  \ you updated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-bridge-output-response-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: UpdateBridgeOutputResponse
---
