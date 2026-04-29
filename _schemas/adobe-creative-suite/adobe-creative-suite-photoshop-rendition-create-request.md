---
description: Request to create one or more renditions from a PSD or image
layout: schema
name: RenditionCreateRequest
properties_list:
- description: ''
  name: inputs
  type: array
- description: List of rendition outputs to generate
  name: outputs
  type: array
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-photoshop-rendition-create-request-schema.json
slug: adobe-creative-suite-photoshop-rendition-create-request
source_filename: adobe-creative-suite-photoshop-rendition-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-rendition-create-request-schema.json\",\n  \"title\": \"RenditionCreateRequest\",\n  \"description\": \"Request to create one or more renditions from a PSD or image\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/JobInput\"\n      }\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"description\": \"List of rendition outputs to generate\",\n      \"items\": {\n        \"type\": \"object\",\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/JobOutput\"\n          },\n          {\n            \"type\": \"object\",\n            \"properties\": {\n              \"quality\": {\n                \"type\": \"integer\",\n  \
  \              \"description\": \"JPEG quality (1-100)\",\n                \"minimum\": 1,\n                \"maximum\": 100\n              },\n              \"compression\": {\n                \"type\": \"string\",\n                \"description\": \"PNG compression level\",\n                \"enum\": [\n                  \"small\",\n                  \"medium\",\n                  \"large\"\n                ]\n              }\n            }\n          }\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"inputs\",\n    \"outputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-rendition-create-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: RenditionCreateRequest
---
