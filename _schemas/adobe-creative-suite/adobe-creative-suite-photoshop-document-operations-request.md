---
description: Request to apply document-level operations to a PSD
layout: schema
name: DocumentOperationsRequest
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
schema_file: json-schema/adobe-creative-suite-photoshop-document-operations-request-schema.json
slug: adobe-creative-suite-photoshop-document-operations-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-document-operations-request-schema.json\",\n  \"title\": \"DocumentOperationsRequest\",\n  \"description\": \"Request to apply document-level operations to a PSD\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/JobInput\"\n      }\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/JobOutput\"\n      }\n    },\n    \"options\": {\n      \"$ref\": \"#/components/schemas/DocumentOperations\"\n    }\n  },\n  \"required\": [\n    \"inputs\",\n    \"outputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-document-operations-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: DocumentOperationsRequest
---
