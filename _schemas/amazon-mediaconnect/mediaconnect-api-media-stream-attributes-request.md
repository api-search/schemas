---
description: Attributes that are related to the media stream.
layout: schema
name: MediaStreamAttributesRequest
properties_list:
- description: ''
  name: Fmtp
  type: object
- description: ''
  name: Lang
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-media-stream-attributes-request-schema.json
slug: mediaconnect-api-media-stream-attributes-request
source_filename: mediaconnect-api-media-stream-attributes-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-media-stream-attributes-request-schema.json\",\n  \"title\": \"MediaStreamAttributesRequest\",\n  \"description\": \"Attributes that are related to the media stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Fmtp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FmtpRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fmtp\"\n          },\n          \"description\": \"The settings that you want to use to define the media stream.\"\n        }\n      ]\n    },\n    \"Lang\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"lang\"\n          },\n          \"description\": \"The audio language, in a format that\
  \ is recognized by the receiver.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-media-stream-attributes-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: MediaStreamAttributesRequest
---
