---
description: Request body for compressing a PDF
layout: schema
name: CompressPDFRequest
properties_list:
- description: Asset ID of the PDF to compress
  name: assetID
  type: string
- description: Compression level to apply
  name: compressionLevel
  type: string
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-pdf-services-compress-pdf-request-schema.json
slug: adobe-creative-suite-pdf-services-compress-pdf-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-compress-pdf-request-schema.json\",\n  \"title\": \"CompressPDFRequest\",\n  \"description\": \"Request body for compressing a PDF\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"Asset ID of the PDF to compress\",\n      \"example\": \"urn:aaid:AS:UE1:23c30ee0-2e4d-46d6-87f2-087832fca718\"\n    },\n    \"compressionLevel\": {\n      \"type\": \"string\",\n      \"description\": \"Compression level to apply\",\n      \"enum\": [\n        \"LOW\",\n        \"MEDIUM\",\n        \"HIGH\"\n      ],\n      \"default\": \"MEDIUM\",\n      \"example\": \"LOW\"\n    }\n  },\n  \"required\": [\n    \"assetID\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-compress-pdf-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: CompressPDFRequest
---
