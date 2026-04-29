---
description: Reference to an output file location in cloud storage
layout: schema
name: JobOutput
properties_list:
- description: URL or path where the output file will be stored
  name: href
  type: string
- description: Cloud storage provider type
  name: storage
  type: string
- description: MIME type of the output file
  name: type
  type: string
- description: Output width in pixels
  name: width
  type: integer
- description: Output height in pixels
  name: height
  type: integer
- description: Whether to overwrite the output file if it already exists
  name: overwrite
  type: boolean
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-photoshop-job-output-schema.json
slug: adobe-creative-suite-photoshop-job-output
source_filename: adobe-creative-suite-photoshop-job-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-job-output-schema.json\",\n  \"title\": \"JobOutput\",\n  \"description\": \"Reference to an output file location in cloud storage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"href\": {\n      \"type\": \"string\",\n      \"description\": \"URL or path where the output file will be stored\",\n      \"example\": \"https://my-storage.blob.core.windows.net/images/output.png\"\n    },\n    \"storage\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud storage provider type\",\n      \"enum\": [\n        \"adobe\",\n        \"external\",\n        \"azure\",\n        \"dropbox\"\n      ],\n      \"example\": \"external\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"MIME type of the output file\",\n      \"example\"\
  : \"image/png\"\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"Output width in pixels\",\n      \"example\": 1920\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"description\": \"Output height in pixels\",\n      \"example\": 1080\n    },\n    \"overwrite\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to overwrite the output file if it already exists\",\n      \"default\": true,\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"href\",\n    \"storage\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-job-output-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: JobOutput
---
