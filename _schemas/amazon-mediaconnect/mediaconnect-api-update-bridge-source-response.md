---
description: UpdateBridgeSourceResponse schema from AWS Elemental MediaConnect API
layout: schema
name: UpdateBridgeSourceResponse
properties_list:
- description: ''
  name: BridgeArn
  type: object
- description: ''
  name: Source
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-update-bridge-source-response-schema.json
slug: mediaconnect-api-update-bridge-source-response
source_filename: mediaconnect-api-update-bridge-source-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-bridge-source-response-schema.json\",\n  \"title\": \"UpdateBridgeSourceResponse\",\n  \"description\": \"UpdateBridgeSourceResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BridgeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bridgeArn\"\n          },\n          \"description\": \"The Amazon Resource Number (ARN) of the bridge.\"\n        }\n      ]\n    },\n    \"Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BridgeSource\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"source\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-bridge-source-response-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: UpdateBridgeSourceResponse
---
