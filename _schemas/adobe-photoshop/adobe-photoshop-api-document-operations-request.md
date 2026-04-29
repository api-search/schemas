---
description: DocumentOperationsRequest from Adobe Photoshop API
layout: schema
name: DocumentOperationsRequest
properties_list:
- description: ''
  name: inputs
  type: array
- description: ''
  name: options
  type: object
- description: ''
  name: outputs
  type: array
provider_name: Adobe Photoshop
provider_slug: adobe-photoshop
schema_file: json-schema/adobe-photoshop-api-document-operations-request-schema.json
slug: adobe-photoshop-api-document-operations-request
source_filename: adobe-photoshop-api-document-operations-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-document-operations-request-schema.json\",\n  \"title\": \"DocumentOperationsRequest\",\n  \"description\": \"DocumentOperationsRequest from Adobe Photoshop API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StorageInput\"\n      }\n    },\n    \"options\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"layers\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/LayerOperation\"\n          }\n        }\n      }\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StorageOutput\"\n      }\n    }\n  },\n  \"required\": [\n    \"inputs\",\n\
  \    \"outputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-document-operations-request-schema.json
tags:
- AI/ML
- Creative Cloud
- Image Editing
- Photoshop
- Plugins
- REST API
- Scripting
title: DocumentOperationsRequest
---
