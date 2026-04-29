---
description: SmartObjectRequest from Adobe Photoshop API
layout: schema
name: SmartObjectRequest
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
schema_file: json-schema/adobe-photoshop-api-smart-object-request-schema.json
slug: adobe-photoshop-api-smart-object-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-smart-object-request-schema.json\",\n  \"title\": \"SmartObjectRequest\",\n  \"description\": \"SmartObjectRequest from Adobe Photoshop API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StorageInput\"\n      }\n    },\n    \"options\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"layers\"\n      ],\n      \"properties\": {\n        \"layers\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"Layer name to target.\"\n              },\n              \"id\": {\n                \"type\"\
  : \"integer\",\n                \"description\": \"Layer ID to target.\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"const\": \"smartObject\"\n              },\n              \"input\": {\n                \"$ref\": \"#/components/schemas/StorageInput\"\n              },\n              \"smartObject\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"type\": {\n                    \"type\": \"string\",\n                    \"description\": \"MIME type of the replacement content.\"\n                  }\n                }\n              },\n              \"attributes\": {\n                \"$ref\": \"#/components/schemas/LayerBounds\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StorageOutput\"\n      }\n    }\n  },\n  \"required\": [\n    \"inputs\"\
  ,\n    \"options\",\n    \"outputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-smart-object-request-schema.json
tags:
- AI/ML
- Creative Cloud
- Image Editing
- Photoshop
- Plugins
- REST API
- Scripting
title: SmartObjectRequest
---
