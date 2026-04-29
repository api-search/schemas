---
description: RemoveFlowOutputResponse schema from AWS Elemental MediaConnect API
layout: schema
name: RemoveFlowOutputResponse
properties_list:
- description: ''
  name: FlowArn
  type: object
- description: ''
  name: OutputArn
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-remove-flow-output-response-schema.json
slug: mediaconnect-api-remove-flow-output-response
source_filename: mediaconnect-api-remove-flow-output-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-remove-flow-output-response-schema.json\",\n  \"title\": \"RemoveFlowOutputResponse\",\n  \"description\": \"RemoveFlowOutputResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlowArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowArn\"\n          },\n          \"description\": \"The ARN of the flow that is associated with the output you removed.\"\n        }\n      ]\n    },\n    \"OutputArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputArn\"\n          },\n          \"description\": \"The\
  \ ARN of the output that was removed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-remove-flow-output-response-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: RemoveFlowOutputResponse
---
