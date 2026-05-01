---
description: Messages that provide the state of the flow.
layout: schema
name: Messages
properties_list:
- description: ''
  name: Errors
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-messages-schema.json
slug: mediaconnect-api-messages
source_filename: mediaconnect-api-messages-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-messages-schema.json\",\n  \"title\": \"Messages\",\n  \"description\": \"Messages that provide the state of the flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"errors\"\n          },\n          \"description\": \"A list of errors that might have been generated from processes on this flow.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Errors\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-messages-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: Messages
---
