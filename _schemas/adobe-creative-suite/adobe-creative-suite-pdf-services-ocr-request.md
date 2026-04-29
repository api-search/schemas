---
description: Request body for applying OCR to a PDF
layout: schema
name: OCRRequest
properties_list:
- description: Asset ID of the scanned PDF to OCR
  name: assetID
  type: string
- description: BCP 47 locale for OCR language model selection
  name: ocrLang
  type: string
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-pdf-services-ocr-request-schema.json
slug: adobe-creative-suite-pdf-services-ocr-request
source_filename: adobe-creative-suite-pdf-services-ocr-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-ocr-request-schema.json\",\n  \"title\": \"OCRRequest\",\n  \"description\": \"Request body for applying OCR to a PDF\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"Asset ID of the scanned PDF to OCR\",\n      \"example\": \"urn:aaid:AS:UE1:23c30ee0-2e4d-46d6-87f2-087832fca718\"\n    },\n    \"ocrLang\": {\n      \"type\": \"string\",\n      \"description\": \"BCP 47 locale for OCR language model selection\",\n      \"example\": \"en-US\"\n    }\n  },\n  \"required\": [\n    \"assetID\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-ocr-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: OCRRequest
---
