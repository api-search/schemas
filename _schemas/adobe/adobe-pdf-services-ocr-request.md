---
description: ''
layout: schema
name: OCRRequest
properties_list:
- description: The asset ID of the PDF to OCR.
  name: assetID
  type: string
- description: The language for OCR processing.
  name: ocrLanguage
  type: string
- description: The type of OCR output. SEARCHABLE_IMAGE produces a searchable PDF maintaining visual fidelity. SEARCHABLE_IMAGE_EXACT preserves the original image appearance precisely.
  name: ocrType
  type: string
provider_name: Adobe
provider_slug: adobe
schema_file: json-schema/adobe-pdf-services-ocr-request-schema.json
slug: adobe-pdf-services-ocr-request
source_filename: adobe-pdf-services-ocr-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OCRRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"The asset ID of the PDF to OCR.\"\n    },\n    \"ocrLanguage\": {\n      \"type\": \"string\",\n      \"description\": \"The language for OCR processing.\"\n    },\n    \"ocrType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of OCR output. SEARCHABLE_IMAGE produces a searchable PDF maintaining visual fidelity. SEARCHABLE_IMAGE_EXACT preserves the original image appearance precisely.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/json-schema/adobe-pdf-services-ocr-request-schema.json
tags:
- Analytics
- Creative Cloud
- Digital Asset Management
- Document Services
- E-Commerce
- E-Signatures
- Experience Cloud
- Generative AI
- Marketing
- PDF
- Work Management
title: OCRRequest
---
