---
description: Request to read or modify layers within a PSD document
layout: schema
name: LayerManageRequest
properties_list:
- description: ''
  name: inputs
  type: array
- description: ''
  name: outputs
  type: array
- description: ''
  name: options
  type: object
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-photoshop-layer-manage-request-schema.json
slug: adobe-creative-suite-photoshop-layer-manage-request
source_filename: adobe-creative-suite-photoshop-layer-manage-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-layer-manage-request-schema.json\",\n  \"title\": \"LayerManageRequest\",\n  \"description\": \"Request to read or modify layers within a PSD document\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/JobInput\"\n      }\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/JobOutput\"\n      }\n    },\n    \"options\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"layers\": {\n          \"type\": \"array\",\n          \"description\": \"Layer operations to apply\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/Layer\"\n          }\n        }\n      }\n\
  \    }\n  },\n  \"required\": [\n    \"inputs\",\n    \"outputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-layer-manage-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: LayerManageRequest
---
