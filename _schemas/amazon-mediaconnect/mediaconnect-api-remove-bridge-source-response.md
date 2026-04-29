---
description: RemoveBridgeSourceResponse schema from AWS Elemental MediaConnect API
layout: schema
name: RemoveBridgeSourceResponse
properties_list:
- description: ''
  name: BridgeArn
  type: object
- description: ''
  name: SourceName
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-remove-bridge-source-response-schema.json
slug: mediaconnect-api-remove-bridge-source-response
source_filename: mediaconnect-api-remove-bridge-source-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-remove-bridge-source-response-schema.json\",\n  \"title\": \"RemoveBridgeSourceResponse\",\n  \"description\": \"RemoveBridgeSourceResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BridgeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bridgeArn\"\n          }\n        }\n      ]\n    },\n    \"SourceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceName\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-remove-bridge-source-response-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: RemoveBridgeSourceResponse
---
