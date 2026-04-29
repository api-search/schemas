---
description: The VPC interface that is used for the media stream associated with the source or output.
layout: schema
name: Interface
properties_list:
- description: ''
  name: Name
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-interface-schema.json
slug: mediaconnect-api-interface
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-interface-schema.json\",\n  \"title\": \"Interface\",\n  \"description\": \"The VPC interface that is used for the media stream associated with the source or output.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the VPC interface.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-interface-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: Interface
---
