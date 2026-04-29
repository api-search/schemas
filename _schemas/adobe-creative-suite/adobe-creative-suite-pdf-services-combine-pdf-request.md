---
description: Request body for combining multiple PDFs
layout: schema
name: CombinePDFRequest
properties_list:
- description: Ordered list of PDF assets to combine
  name: assets
  type: array
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-pdf-services-combine-pdf-request-schema.json
slug: adobe-creative-suite-pdf-services-combine-pdf-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-combine-pdf-request-schema.json\",\n  \"title\": \"CombinePDFRequest\",\n  \"description\": \"Request body for combining multiple PDFs\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assets\": {\n      \"type\": \"array\",\n      \"description\": \"Ordered list of PDF assets to combine\",\n      \"minItems\": 2,\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\n          \"assetID\"\n        ],\n        \"properties\": {\n          \"assetID\": {\n            \"type\": \"string\",\n            \"description\": \"Asset ID of the PDF to include\"\n          },\n          \"pageRanges\": {\n            \"type\": \"array\",\n            \"description\": \"Optional page ranges to extract from this PDF\",\n            \"items\": {\n  \
  \            \"$ref\": \"#/components/schemas/PageRange\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"assets\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-combine-pdf-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: CombinePDFRequest
---
