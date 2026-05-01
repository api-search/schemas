---
description: A request to add outputs to the specified bridge.
layout: schema
name: AddBridgeOutputsRequest
properties_list:
- description: ''
  name: Outputs
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-add-bridge-outputs-request-schema.json
slug: mediaconnect-api-add-bridge-outputs-request
source_filename: mediaconnect-api-add-bridge-outputs-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-bridge-outputs-request-schema.json\",\n  \"title\": \"AddBridgeOutputsRequest\",\n  \"description\": \"A request to add outputs to the specified bridge.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Outputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfAddBridgeOutputRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputs\"\n          },\n          \"description\": \"The outputs that you want to add to this bridge.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Outputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-bridge-outputs-request-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: AddBridgeOutputsRequest
---
