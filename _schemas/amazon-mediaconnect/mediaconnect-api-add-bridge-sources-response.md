---
description: AddBridgeSourcesResponse schema from AWS Elemental MediaConnect API
layout: schema
name: AddBridgeSourcesResponse
properties_list:
- description: ''
  name: BridgeArn
  type: object
- description: ''
  name: Sources
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-add-bridge-sources-response-schema.json
slug: mediaconnect-api-add-bridge-sources-response
source_filename: mediaconnect-api-add-bridge-sources-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-bridge-sources-response-schema.json\",\n  \"title\": \"AddBridgeSourcesResponse\",\n  \"description\": \"AddBridgeSourcesResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BridgeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bridgeArn\"\n          },\n          \"description\": \"The Amazon Resource Number (ARN) of the bridge.\"\n        }\n      ]\n    },\n    \"Sources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfBridgeSource\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sources\"\n          },\n          \"description\": \"The sources\
  \ that you added to this bridge.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-bridge-sources-response-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: AddBridgeSourcesResponse
---
