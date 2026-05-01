---
description: A request to update flow.
layout: schema
name: UpdateFlowRequest
properties_list:
- description: ''
  name: SourceFailoverConfig
  type: object
- description: ''
  name: Maintenance
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-update-flow-request-schema.json
slug: mediaconnect-api-update-flow-request
source_filename: mediaconnect-api-update-flow-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-flow-request-schema.json\",\n  \"title\": \"UpdateFlowRequest\",\n  \"description\": \"A request to update flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceFailoverConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateFailoverConfig\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceFailoverConfig\"\n          }\n        }\n      ]\n    },\n    \"Maintenance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateMaintenance\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenance\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-flow-request-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: UpdateFlowRequest
---
