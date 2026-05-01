---
description: Displays details of the selected bridge.
layout: schema
name: ListedBridge
properties_list:
- description: ''
  name: BridgeArn
  type: object
- description: ''
  name: BridgeState
  type: object
- description: ''
  name: BridgeType
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: PlacementArn
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-listed-bridge-schema.json
slug: mediaconnect-api-listed-bridge
source_filename: mediaconnect-api-listed-bridge-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-listed-bridge-schema.json\",\n  \"title\": \"ListedBridge\",\n  \"description\": \"Displays details of the selected bridge.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BridgeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bridgeArn\"\n          },\n          \"description\": \"The ARN of the bridge.\"\n        }\n      ]\n    },\n    \"BridgeState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BridgeState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bridgeState\"\n          }\n        }\n      ]\n    },\n    \"BridgeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"bridgeType\"\n          },\n          \"description\": \"The type of the bridge.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the bridge.\"\n        }\n      ]\n    },\n    \"PlacementArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"placementArn\"\n          },\n          \"description\": \"The ARN of the gateway associated with the bridge.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BridgeArn\",\n    \"BridgeState\",\n    \"PlacementArn\",\n    \"BridgeType\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-listed-bridge-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: ListedBridge
---
