---
description: RemoveBridgeOutputResponse schema from AWS Elemental MediaConnect API
layout: schema
name: RemoveBridgeOutputResponse
properties_list:
- description: ''
  name: BridgeArn
  type: object
- description: ''
  name: OutputName
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-remove-bridge-output-response-schema.json
slug: mediaconnect-api-remove-bridge-output-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-remove-bridge-output-response-schema.json\",\n  \"title\": \"RemoveBridgeOutputResponse\",\n  \"description\": \"RemoveBridgeOutputResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BridgeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bridgeArn\"\n          }\n        }\n      ]\n    },\n    \"OutputName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputName\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-remove-bridge-output-response-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: RemoveBridgeOutputResponse
---
