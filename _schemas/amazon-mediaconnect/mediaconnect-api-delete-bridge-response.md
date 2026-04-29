---
description: DeleteBridgeResponse schema from AWS Elemental MediaConnect API
layout: schema
name: DeleteBridgeResponse
properties_list:
- description: ''
  name: BridgeArn
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-delete-bridge-response-schema.json
slug: mediaconnect-api-delete-bridge-response
source_filename: mediaconnect-api-delete-bridge-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-delete-bridge-response-schema.json\",\n  \"title\": \"DeleteBridgeResponse\",\n  \"description\": \"DeleteBridgeResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BridgeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bridgeArn\"\n          },\n          \"description\": \"The Amazon Resource Number (ARN) of the deleted bridge.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-delete-bridge-response-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: DeleteBridgeResponse
---
