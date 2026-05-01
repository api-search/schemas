---
description: AddFlowSourcesResponse schema from AWS Elemental MediaConnect API
layout: schema
name: AddFlowSourcesResponse
properties_list:
- description: ''
  name: FlowArn
  type: object
- description: ''
  name: Sources
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-add-flow-sources-response-schema.json
slug: mediaconnect-api-add-flow-sources-response
source_filename: mediaconnect-api-add-flow-sources-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-flow-sources-response-schema.json\",\n  \"title\": \"AddFlowSourcesResponse\",\n  \"description\": \"AddFlowSourcesResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlowArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowArn\"\n          },\n          \"description\": \"The ARN of the flow that these sources were added to.\"\n        }\n      ]\n    },\n    \"Sources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfSource\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sources\"\n          },\n          \"description\": \"The details of the newly\
  \ added sources.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-flow-sources-response-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: AddFlowSourcesResponse
---
