---
description: Request to create an alpha mask for an image
layout: schema
name: MaskRequest
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
schema_file: json-schema/adobe-creative-suite-photoshop-mask-request-schema.json
slug: adobe-creative-suite-photoshop-mask-request
source_filename: adobe-creative-suite-photoshop-mask-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-mask-request-schema.json\",\n  \"title\": \"MaskRequest\",\n  \"description\": \"Request to create an alpha mask for an image\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"input\": {\n      \"$ref\": \"#/components/schemas/JobInput\"\n    },\n    \"output\": {\n      \"$ref\": \"#/components/schemas/JobOutput\"\n    },\n    \"options\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"optimize\": {\n          \"type\": \"string\",\n          \"description\": \"Optimization mode for mask generation\",\n          \"enum\": [\n            \"performance\",\n            \"batch\"\n          ]\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"input\",\n    \"output\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-mask-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: MaskRequest
---
