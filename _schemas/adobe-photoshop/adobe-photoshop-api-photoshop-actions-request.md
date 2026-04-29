---
description: PhotoshopActionsRequest from Adobe Photoshop API
layout: schema
name: PhotoshopActionsRequest
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
schema_file: json-schema/adobe-photoshop-api-photoshop-actions-request-schema.json
slug: adobe-photoshop-api-photoshop-actions-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-photoshop-actions-request-schema.json\",\n  \"title\": \"PhotoshopActionsRequest\",\n  \"description\": \"PhotoshopActionsRequest from Adobe Photoshop API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StorageInput\"\n      }\n    },\n    \"options\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"actions\"\n      ],\n      \"properties\": {\n        \"actions\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"required\": [\n              \"href\",\n              \"storage\"\n            ],\n            \"properties\": {\n              \"href\": {\n                \"type\": \"string\",\n         \
  \       \"description\": \"URL to the .atn Action file.\"\n              },\n              \"storage\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"external\",\n                  \"adobe\",\n                  \"azure\",\n                  \"dropbox\"\n                ]\n              },\n              \"actionName\": {\n                \"type\": \"string\",\n                \"description\": \"Specific action name to run within the set.\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StorageOutput\"\n      }\n    }\n  },\n  \"required\": [\n    \"inputs\",\n    \"options\",\n    \"outputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-photoshop-actions-request-schema.json
tags:
- AI/ML
- Creative Cloud
- Image Editing
- Photoshop
- Plugins
- REST API
- Scripting
title: PhotoshopActionsRequest
---
