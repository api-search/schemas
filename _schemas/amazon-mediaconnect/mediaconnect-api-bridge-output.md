---
description: The output of the bridge.
layout: schema
name: BridgeOutput
properties_list:
- description: ''
  name: FlowOutput
  type: object
- description: ''
  name: NetworkOutput
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-bridge-output-schema.json
slug: mediaconnect-api-bridge-output
source_filename: mediaconnect-api-bridge-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-bridge-output-schema.json\",\n  \"title\": \"BridgeOutput\",\n  \"description\": \"The output of the bridge.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlowOutput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BridgeFlowOutput\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowOutput\"\n          }\n        }\n      ]\n    },\n    \"NetworkOutput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BridgeNetworkOutput\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkOutput\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-bridge-output-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: BridgeOutput
---
