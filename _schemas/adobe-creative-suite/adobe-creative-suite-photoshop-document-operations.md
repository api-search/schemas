---
description: Operations to apply to a PSD document
layout: schema
name: DocumentOperations
properties_list:
- description: Resize the document canvas or image
  name: resize
  type: object
- description: Whether to flatten all layers into a single layer
  name: flatten
  type: boolean
- description: Trim transparent borders from the image
  name: trim
  type: object
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-photoshop-document-operations-schema.json
slug: adobe-creative-suite-photoshop-document-operations
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-document-operations-schema.json\",\n  \"title\": \"DocumentOperations\",\n  \"description\": \"Operations to apply to a PSD document\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resize\": {\n      \"type\": \"object\",\n      \"description\": \"Resize the document canvas or image\",\n      \"properties\": {\n        \"width\": {\n          \"type\": \"integer\"\n        },\n        \"height\": {\n          \"type\": \"integer\"\n        },\n        \"unit\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"pixel\",\n            \"percent\"\n          ]\n        },\n        \"resampleMethod\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"bicubic\",\n            \"bilinear\",\n            \"nearestNeighbor\"\
  ,\n            \"preserve\"\n          ]\n        }\n      }\n    },\n    \"flatten\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to flatten all layers into a single layer\",\n      \"example\": true\n    },\n    \"trim\": {\n      \"type\": \"object\",\n      \"description\": \"Trim transparent borders from the image\",\n      \"properties\": {\n        \"basedOn\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"transparentPixels\",\n            \"topLeftPixelColor\",\n            \"bottomRightPixelColor\"\n          ]\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-document-operations-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: DocumentOperations
---
