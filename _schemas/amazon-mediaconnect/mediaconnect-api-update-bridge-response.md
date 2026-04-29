---
description: UpdateBridgeResponse schema from AWS Elemental MediaConnect API
layout: schema
name: UpdateBridgeResponse
properties_list:
- description: ''
  name: Bridge
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-update-bridge-response-schema.json
slug: mediaconnect-api-update-bridge-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-bridge-response-schema.json\",\n  \"title\": \"UpdateBridgeResponse\",\n  \"description\": \"UpdateBridgeResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bridge\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Bridge\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bridge\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-bridge-response-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: UpdateBridgeResponse
---
