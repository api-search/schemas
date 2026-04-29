---
description: The transport parameters that you want to associate with an incoming media stream.
layout: schema
name: InputConfigurationRequest
properties_list:
- description: ''
  name: InputPort
  type: object
- description: ''
  name: Interface
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-input-configuration-request-schema.json
slug: mediaconnect-api-input-configuration-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-input-configuration-request-schema.json\",\n  \"title\": \"InputConfigurationRequest\",\n  \"description\": \"The transport parameters that you want to associate with an incoming media stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputPort\"\n          },\n          \"description\": \"The port that you want the flow to listen on for an incoming media stream.\"\n        }\n      ]\n    },\n    \"Interface\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InterfaceRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"interface\"\n          },\n\
  \          \"description\": \"The VPC interface that you want to use for the incoming media stream.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InputPort\",\n    \"Interface\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-input-configuration-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: InputConfigurationRequest
---
