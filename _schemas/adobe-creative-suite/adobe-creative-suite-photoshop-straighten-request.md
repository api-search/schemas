---
description: Request to automatically straighten an image
layout: schema
name: StraightenRequest
properties_list:
- description: ''
  name: input
  type: object
- description: ''
  name: output
  type: object
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-photoshop-straighten-request-schema.json
slug: adobe-creative-suite-photoshop-straighten-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-straighten-request-schema.json\",\n  \"title\": \"StraightenRequest\",\n  \"description\": \"Request to automatically straighten an image\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"input\": {\n      \"$ref\": \"#/components/schemas/JobInput\"\n    },\n    \"output\": {\n      \"$ref\": \"#/components/schemas/JobOutput\"\n    }\n  },\n  \"required\": [\n    \"input\",\n    \"output\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-straighten-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: StraightenRequest
---
