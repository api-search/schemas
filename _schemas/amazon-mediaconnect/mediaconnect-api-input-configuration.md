---
description: The transport parameters that are associated with an incoming media stream.
layout: schema
name: InputConfiguration
properties_list:
- description: ''
  name: InputIp
  type: object
- description: ''
  name: InputPort
  type: object
- description: ''
  name: Interface
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-input-configuration-schema.json
slug: mediaconnect-api-input-configuration
source_filename: mediaconnect-api-input-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-input-configuration-schema.json\",\n  \"title\": \"InputConfiguration\",\n  \"description\": \"The transport parameters that are associated with an incoming media stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputIp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputIp\"\n          },\n          \"description\": \"The IP address that the flow listens on for incoming content for a media stream.\"\n        }\n      ]\n    },\n    \"InputPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputPort\"\n          },\n          \"description\"\
  : \"The port that the flow listens on for an incoming media stream.\"\n        }\n      ]\n    },\n    \"Interface\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Interface\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"interface\"\n          },\n          \"description\": \"The VPC interface where the media stream comes in from.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InputPort\",\n    \"InputIp\",\n    \"Interface\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-input-configuration-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: InputConfiguration
---
