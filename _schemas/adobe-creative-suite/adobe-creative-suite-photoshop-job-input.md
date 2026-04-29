---
description: Reference to an input file stored in cloud storage
layout: schema
name: JobInput
properties_list:
- description: URL or path to the input file in cloud storage
  name: href
  type: string
- description: Cloud storage provider type
  name: storage
  type: string
- description: MIME type of the input file
  name: type
  type: string
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-photoshop-job-input-schema.json
slug: adobe-creative-suite-photoshop-job-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-job-input-schema.json\",\n  \"title\": \"JobInput\",\n  \"description\": \"Reference to an input file stored in cloud storage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"href\": {\n      \"type\": \"string\",\n      \"description\": \"URL or path to the input file in cloud storage\",\n      \"example\": \"https://my-storage.blob.core.windows.net/images/input.psd\"\n    },\n    \"storage\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud storage provider type\",\n      \"enum\": [\n        \"adobe\",\n        \"external\",\n        \"azure\",\n        \"dropbox\"\n      ],\n      \"example\": \"external\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"MIME type of the input file\",\n      \"example\": \"image/vnd.adobe.photoshop\"\
  \n    }\n  },\n  \"required\": [\n    \"href\",\n    \"storage\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-job-input-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: JobInput
---
