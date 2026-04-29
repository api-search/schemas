---
description: A request to add sources to the flow.
layout: schema
name: AddFlowSourcesRequest
properties_list:
- description: ''
  name: Sources
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-add-flow-sources-request-schema.json
slug: mediaconnect-api-add-flow-sources-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-flow-sources-request-schema.json\",\n  \"title\": \"AddFlowSourcesRequest\",\n  \"description\": \"A request to add sources to the flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Sources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfSetSourceRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sources\"\n          },\n          \"description\": \"A list of sources that you want to add.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Sources\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-flow-sources-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: AddFlowSourcesRequest
---
