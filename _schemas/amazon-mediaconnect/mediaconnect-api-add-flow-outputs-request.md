---
description: A request to add outputs to the specified flow.
layout: schema
name: AddFlowOutputsRequest
properties_list:
- description: ''
  name: Outputs
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-add-flow-outputs-request-schema.json
slug: mediaconnect-api-add-flow-outputs-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-flow-outputs-request-schema.json\",\n  \"title\": \"AddFlowOutputsRequest\",\n  \"description\": \"A request to add outputs to the specified flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Outputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfAddOutputRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputs\"\n          },\n          \"description\": \"A list of outputs that you want to add.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Outputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-flow-outputs-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: AddFlowOutputsRequest
---
