---
description: Request to automatically crop an image to the primary product
layout: schema
name: ProductCropRequest
properties_list:
- description: ''
  name: input
  type: object
- description: ''
  name: output
  type: object
- description: ''
  name: options
  type: object
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-photoshop-product-crop-request-schema.json
slug: adobe-creative-suite-photoshop-product-crop-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-product-crop-request-schema.json\",\n  \"title\": \"ProductCropRequest\",\n  \"description\": \"Request to automatically crop an image to the primary product\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"input\": {\n      \"$ref\": \"#/components/schemas/JobInput\"\n    },\n    \"output\": {\n      \"$ref\": \"#/components/schemas/JobOutput\"\n    },\n    \"options\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"unit\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"pixel\",\n            \"percent\"\n          ]\n        },\n        \"padding\": {\n          \"type\": \"number\",\n          \"description\": \"Padding to add around the product crop\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"input\"\
  ,\n    \"output\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-product-crop-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: ProductCropRequest
---
