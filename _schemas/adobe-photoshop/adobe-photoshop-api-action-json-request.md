---
description: ActionJSONRequest from Adobe Photoshop API
layout: schema
name: ActionJSONRequest
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
schema_file: json-schema/adobe-photoshop-api-action-json-request-schema.json
slug: adobe-photoshop-api-action-json-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-action-json-request-schema.json\",\n  \"title\": \"ActionJSONRequest\",\n  \"description\": \"ActionJSONRequest from Adobe Photoshop API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StorageInput\"\n      }\n    },\n    \"options\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"actionJSON\"\n      ],\n      \"properties\": {\n        \"actionJSON\": {\n          \"type\": \"array\",\n          \"description\": \"Array of Photoshop action descriptor objects.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"required\": [\n              \"_obj\"\n            ],\n            \"properties\": {\n              \"_obj\": {\n         \
  \       \"type\": \"string\",\n                \"description\": \"Photoshop action descriptor type.\"\n              }\n            },\n            \"additionalProperties\": true\n          }\n        },\n        \"additionalImages\": {\n          \"type\": \"array\",\n          \"description\": \"Additional images for compositing, referenced in actionJSON as ACTION_JSON_OPTIONS_ADDITIONAL_IMAGES_0, etc.\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/StorageInput\"\n          }\n        }\n      }\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StorageOutput\"\n      }\n    }\n  },\n  \"required\": [\n    \"options\",\n    \"outputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-action-json-request-schema.json
tags:
- AI/ML
- Creative Cloud
- Image Editing
- Photoshop
- Plugins
- REST API
- Scripting
title: ActionJSONRequest
---
