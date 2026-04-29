---
description: UpdateFlowSourceResponse schema from AWS Elemental MediaConnect API
layout: schema
name: UpdateFlowSourceResponse
properties_list:
- description: ''
  name: FlowArn
  type: object
- description: ''
  name: Source
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-update-flow-source-response-schema.json
slug: mediaconnect-api-update-flow-source-response
source_filename: mediaconnect-api-update-flow-source-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-flow-source-response-schema.json\",\n  \"title\": \"UpdateFlowSourceResponse\",\n  \"description\": \"UpdateFlowSourceResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlowArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowArn\"\n          },\n          \"description\": \"The ARN of the flow that you want to update.\"\n        }\n      ]\n    },\n    \"Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Source\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"source\"\n          },\n          \"description\": \"The settings for the source of the\
  \ flow.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-flow-source-response-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: UpdateFlowSourceResponse
---
