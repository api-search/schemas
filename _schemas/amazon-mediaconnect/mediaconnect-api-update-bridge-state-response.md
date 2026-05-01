---
description: UpdateBridgeStateResponse schema from AWS Elemental MediaConnect API
layout: schema
name: UpdateBridgeStateResponse
properties_list:
- description: ''
  name: BridgeArn
  type: object
- description: ''
  name: DesiredState
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-update-bridge-state-response-schema.json
slug: mediaconnect-api-update-bridge-state-response
source_filename: mediaconnect-api-update-bridge-state-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-bridge-state-response-schema.json\",\n  \"title\": \"UpdateBridgeStateResponse\",\n  \"description\": \"UpdateBridgeStateResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BridgeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bridgeArn\"\n          },\n          \"description\": \"The Amazon Resource Number (ARN) of the bridge.\"\n        }\n      ]\n    },\n    \"DesiredState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DesiredState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"desiredState\"\n          },\n          \"description\": \"The state\
  \ of the bridge. ACTIVE or STANDBY.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-bridge-state-response-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: UpdateBridgeStateResponse
---
