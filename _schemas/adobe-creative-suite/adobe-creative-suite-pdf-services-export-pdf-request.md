---
description: Request body for exporting a PDF to another format
layout: schema
name: ExportPDFRequest
properties_list:
- description: Asset ID of the PDF to export
  name: assetID
  type: string
- description: Target output format for the exported file
  name: targetFormat
  type: string
- description: Locale for OCR during export, if the PDF contains scanned text
  name: exportOCRLocale
  type: string
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-pdf-services-export-pdf-request-schema.json
slug: adobe-creative-suite-pdf-services-export-pdf-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-export-pdf-request-schema.json\",\n  \"title\": \"ExportPDFRequest\",\n  \"description\": \"Request body for exporting a PDF to another format\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"Asset ID of the PDF to export\",\n      \"example\": \"urn:aaid:AS:UE1:23c30ee0-2e4d-46d6-87f2-087832fca718\"\n    },\n    \"targetFormat\": {\n      \"type\": \"string\",\n      \"description\": \"Target output format for the exported file\",\n      \"enum\": [\n        \"docx\",\n        \"xlsx\",\n        \"pptx\",\n        \"rtf\",\n        \"txt\"\n      ],\n      \"example\": \"docx\"\n    },\n    \"exportOCRLocale\": {\n      \"type\": \"string\",\n      \"description\": \"Locale for OCR during\
  \ export, if the PDF contains scanned text\",\n      \"example\": \"en-US\"\n    }\n  },\n  \"required\": [\n    \"assetID\",\n    \"targetFormat\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-export-pdf-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: ExportPDFRequest
---
