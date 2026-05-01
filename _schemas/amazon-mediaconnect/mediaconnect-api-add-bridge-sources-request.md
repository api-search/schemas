---
description: A request to add sources to the specified bridge.
layout: schema
name: AddBridgeSourcesRequest
properties_list:
- description: ''
  name: Sources
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-add-bridge-sources-request-schema.json
slug: mediaconnect-api-add-bridge-sources-request
source_filename: mediaconnect-api-add-bridge-sources-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-bridge-sources-request-schema.json\",\n  \"title\": \"AddBridgeSourcesRequest\",\n  \"description\": \"A request to add sources to the specified bridge.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Sources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfAddBridgeSourceRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sources\"\n          },\n          \"description\": \"The sources that you want to add to this bridge.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Sources\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-bridge-sources-request-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: AddBridgeSourcesRequest
---
