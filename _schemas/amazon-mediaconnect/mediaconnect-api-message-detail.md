---
description: MessageDetail schema from AWS Elemental MediaConnect API
layout: schema
name: MessageDetail
properties_list:
- description: ''
  name: Code
  type: object
- description: ''
  name: Message
  type: object
- description: ''
  name: ResourceName
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-message-detail-schema.json
slug: mediaconnect-api-message-detail
source_filename: mediaconnect-api-message-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-message-detail-schema.json\",\n  \"title\": \"MessageDetail\",\n  \"description\": \"MessageDetail schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"code\"\n          },\n          \"description\": \"The error code.\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"message\"\n          },\n          \"description\": \"The specific error message that MediaConnect returns to help you understand the reason that the request\
  \ did not succeed.\"\n        }\n      ]\n    },\n    \"ResourceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"resourceName\"\n          },\n          \"description\": \"The name of the resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Message\",\n    \"Code\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-message-detail-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: MessageDetail
---
