---
description: UpdateFlowOutputResponse schema from AWS Elemental MediaConnect API
layout: schema
name: UpdateFlowOutputResponse
properties_list:
- description: ''
  name: FlowArn
  type: object
- description: ''
  name: Output
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-update-flow-output-response-schema.json
slug: mediaconnect-api-update-flow-output-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-flow-output-response-schema.json\",\n  \"title\": \"UpdateFlowOutputResponse\",\n  \"description\": \"UpdateFlowOutputResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlowArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowArn\"\n          },\n          \"description\": \"The ARN of the flow that is associated with the updated output.\"\n        }\n      ]\n    },\n    \"Output\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Output\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"output\"\n          },\n          \"description\": \"The new settings\
  \ of the output that you updated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-flow-output-response-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: UpdateFlowOutputResponse
---
