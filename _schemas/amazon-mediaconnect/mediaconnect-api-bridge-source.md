---
description: The bridge's source.
layout: schema
name: BridgeSource
properties_list:
- description: ''
  name: FlowSource
  type: object
- description: ''
  name: NetworkSource
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-bridge-source-schema.json
slug: mediaconnect-api-bridge-source
source_filename: mediaconnect-api-bridge-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-bridge-source-schema.json\",\n  \"title\": \"BridgeSource\",\n  \"description\": \"The bridge's source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlowSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BridgeFlowSource\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowSource\"\n          }\n        }\n      ]\n    },\n    \"NetworkSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BridgeNetworkSource\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkSource\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-bridge-source-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: BridgeSource
---
