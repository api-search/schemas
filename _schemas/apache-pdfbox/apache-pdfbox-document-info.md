---
description: DocumentInfo schema from Apache PDFBox
layout: schema
name: DocumentInfo
properties_list:
- description: ''
  name: documentId
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: pageCount
  type: integer
- description: ''
  name: fileSize
  type: integer
- description: ''
  name: version
  type: string
provider_name: Apache PDFBox
provider_slug: apache-pdfbox
schema_file: json-schema/apache-pdfbox-document-info-schema.json
slug: apache-pdfbox-document-info
source_filename: apache-pdfbox-document-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pdfbox/refs/heads/main/json-schema/apache-pdfbox-document-info-schema.json\",\n  \"title\": \"DocumentInfo\",\n  \"description\": \"DocumentInfo schema from Apache PDFBox\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"documentId\": {\n      \"type\": \"string\",\n      \"example\": \"doc-abc123\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"example\": \"My Document\"\n    },\n    \"pageCount\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"fileSize\": {\n      \"type\": \"integer\",\n      \"example\": 204800\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"example\": \"1.4\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pdfbox/refs/heads/main/json-schema/apache-pdfbox-document-info-schema.json
tags:
- Document Processing
- Java
- PDF
- Text Extraction
- Apache
- Open Source
title: DocumentInfo
---
