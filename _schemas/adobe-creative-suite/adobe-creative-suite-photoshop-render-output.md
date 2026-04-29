---
description: Details of a rendered output file
layout: schema
name: RenderOutput
properties_list:
- description: Reference to the input file used to produce this output
  name: input
  type: string
- description: Status of this specific output
  name: status
  type: string
- description: Additional detail message for this output
  name: details
  type: string
- description: ''
  name: _links
  type: object
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-photoshop-render-output-schema.json
slug: adobe-creative-suite-photoshop-render-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-render-output-schema.json\",\n  \"title\": \"RenderOutput\",\n  \"description\": \"Details of a rendered output file\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"input\": {\n      \"type\": \"string\",\n      \"description\": \"Reference to the input file used to produce this output\",\n      \"example\": \"example_value\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of this specific output\",\n      \"enum\": [\n        \"pending\",\n        \"running\",\n        \"succeeded\",\n        \"failed\"\n      ],\n      \"example\": \"pending\"\n    },\n    \"details\": {\n      \"type\": \"string\",\n      \"description\": \"Additional detail message for this output\",\n      \"example\": \"example_value\"\n    },\n\
  \    \"_links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"renditions\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"href\": {\n                \"type\": \"string\",\n                \"description\": \"URL of the rendered output file\"\n              },\n              \"storage\": {\n                \"type\": \"string\"\n              },\n              \"type\": {\n                \"type\": \"string\"\n              },\n              \"width\": {\n                \"type\": \"integer\"\n              },\n              \"height\": {\n                \"type\": \"integer\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-render-output-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: RenderOutput
---
