---
description: The fields that you want to update in the bridge source.
layout: schema
name: UpdateBridgeSourceRequest
properties_list:
- description: ''
  name: FlowSource
  type: object
- description: ''
  name: NetworkSource
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-update-bridge-source-request-schema.json
slug: mediaconnect-api-update-bridge-source-request
source_filename: mediaconnect-api-update-bridge-source-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-bridge-source-request-schema.json\",\n  \"title\": \"UpdateBridgeSourceRequest\",\n  \"description\": \"The fields that you want to update in the bridge source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlowSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateBridgeFlowSourceRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowSource\"\n          }\n        }\n      ]\n    },\n    \"NetworkSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateBridgeNetworkSourceRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkSource\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-bridge-source-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: UpdateBridgeSourceRequest
---
