---
description: The VPC interface that you want to designate where the media stream is coming from or going to.
layout: schema
name: InterfaceRequest
properties_list:
- description: ''
  name: Name
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-interface-request-schema.json
slug: mediaconnect-api-interface-request
source_filename: mediaconnect-api-interface-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-interface-request-schema.json\",\n  \"title\": \"InterfaceRequest\",\n  \"description\": \"The VPC interface that you want to designate where the media stream is coming from or going to.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the VPC interface.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-interface-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: InterfaceRequest
---
