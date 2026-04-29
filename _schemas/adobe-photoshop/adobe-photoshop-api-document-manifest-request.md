---
description: DocumentManifestRequest from Adobe Photoshop API
layout: schema
name: DocumentManifestRequest
properties_list:
- description: ''
  name: inputs
  type: array
- description: ''
  name: options
  type: object
provider_name: Adobe Photoshop
provider_slug: adobe-photoshop
schema_file: json-schema/adobe-photoshop-api-document-manifest-request-schema.json
slug: adobe-photoshop-api-document-manifest-request
source_filename: adobe-photoshop-api-document-manifest-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-document-manifest-request-schema.json\",\n  \"title\": \"DocumentManifestRequest\",\n  \"description\": \"DocumentManifestRequest from Adobe Photoshop API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StorageInput\"\n      }\n    },\n    \"options\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"thumbnails\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"image/png\",\n                \"image/jpeg\"\n              ],\n              \"description\": \"Format for layer thumbnails.\"\n            }\n          }\n        }\n      }\n\
  \    }\n  },\n  \"required\": [\n    \"inputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-document-manifest-request-schema.json
tags:
- AI/ML
- Creative Cloud
- Image Editing
- Photoshop
- Plugins
- REST API
- Scripting
title: DocumentManifestRequest
---
