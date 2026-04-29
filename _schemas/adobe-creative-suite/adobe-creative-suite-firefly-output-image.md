---
description: A single generated image output from a Firefly generation job
layout: schema
name: OutputImage
properties_list:
- description: Generated image reference
  name: image
  type: object
- description: Seed value used to produce this particular output
  name: seed
  type: integer
- description: Content class detected or applied during generation
  name: contentClass
  type: string
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-firefly-output-image-schema.json
slug: adobe-creative-suite-firefly-output-image
source_filename: adobe-creative-suite-firefly-output-image-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-output-image-schema.json\",\n  \"title\": \"OutputImage\",\n  \"description\": \"A single generated image output from a Firefly generation job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"image\": {\n      \"type\": \"object\",\n      \"description\": \"Generated image reference\",\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"description\": \"Temporary signed URL to download the generated image\",\n          \"example\": \"https://firefly-api-prod-origin.adobe.io/v2/assets/urn:firefly:image:abc123\"\n        }\n      }\n    },\n    \"seed\": {\n      \"type\": \"integer\",\n      \"description\": \"Seed value used to produce this particular output\",\n      \"example\": 42\n    },\n    \"contentClass\": {\n     \
  \ \"type\": \"string\",\n      \"description\": \"Content class detected or applied during generation\",\n      \"enum\": [\n        \"photo\",\n        \"art\"\n      ],\n      \"example\": \"photo\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-output-image-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: OutputImage
---
