---
description: The fields that you want to update in the bridge output.
layout: schema
name: UpdateBridgeOutputRequest
properties_list:
- description: ''
  name: NetworkOutput
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-update-bridge-output-request-schema.json
slug: mediaconnect-api-update-bridge-output-request
source_filename: mediaconnect-api-update-bridge-output-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-bridge-output-request-schema.json\",\n  \"title\": \"UpdateBridgeOutputRequest\",\n  \"description\": \"The fields that you want to update in the bridge output.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NetworkOutput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateBridgeNetworkOutputRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkOutput\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-bridge-output-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: UpdateBridgeOutputRequest
---
