---
description: A request to update the bridge state.
layout: schema
name: UpdateBridgeStateRequest
properties_list:
- description: ''
  name: DesiredState
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-update-bridge-state-request-schema.json
slug: mediaconnect-api-update-bridge-state-request
source_filename: mediaconnect-api-update-bridge-state-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-bridge-state-request-schema.json\",\n  \"title\": \"UpdateBridgeStateRequest\",\n  \"description\": \"A request to update the bridge state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DesiredState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DesiredState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"desiredState\"\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DesiredState\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-bridge-state-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: UpdateBridgeStateRequest
---
