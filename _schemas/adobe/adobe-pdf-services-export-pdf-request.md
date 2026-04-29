---
description: ''
layout: schema
name: ExportPDFRequest
properties_list:
- description: The asset ID of the PDF to export.
  name: assetID
  type: string
- description: The desired output format.
  name: targetFormat
  type: string
- description: The language for OCR processing during export.
  name: ocrLanguage
  type: string
provider_name: Adobe
provider_slug: adobe
schema_file: json-schema/adobe-pdf-services-export-pdf-request-schema.json
slug: adobe-pdf-services-export-pdf-request
source_filename: adobe-pdf-services-export-pdf-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExportPDFRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"The asset ID of the PDF to export.\"\n    },\n    \"targetFormat\": {\n      \"type\": \"string\",\n      \"description\": \"The desired output format.\"\n    },\n    \"ocrLanguage\": {\n      \"type\": \"string\",\n      \"description\": \"The language for OCR processing during export.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/json-schema/adobe-pdf-services-export-pdf-request-schema.json
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
title: ExportPDFRequest
---
