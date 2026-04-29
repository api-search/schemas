---
description: UpdateFlowResponse schema from AWS Elemental MediaConnect API
layout: schema
name: UpdateFlowResponse
properties_list:
- description: ''
  name: Flow
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-update-flow-response-schema.json
slug: mediaconnect-api-update-flow-response
source_filename: mediaconnect-api-update-flow-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-flow-response-schema.json\",\n  \"title\": \"UpdateFlowResponse\",\n  \"description\": \"UpdateFlowResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Flow\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Flow\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flow\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-flow-response-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: UpdateFlowResponse
---
