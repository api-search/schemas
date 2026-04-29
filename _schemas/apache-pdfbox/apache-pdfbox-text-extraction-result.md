---
description: TextExtractionResult schema from Apache PDFBox
layout: schema
name: TextExtractionResult
properties_list:
- description: ''
  name: documentId
  type: string
- description: ''
  name: text
  type: string
- description: ''
  name: pageCount
  type: integer
- description: ''
  name: wordCount
  type: integer
provider_name: Apache PDFBox
provider_slug: apache-pdfbox
schema_file: json-schema/apache-pdfbox-text-extraction-result-schema.json
slug: apache-pdfbox-text-extraction-result
source_filename: apache-pdfbox-text-extraction-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pdfbox/refs/heads/main/json-schema/apache-pdfbox-text-extraction-result-schema.json\",\n  \"title\": \"TextExtractionResult\",\n  \"description\": \"TextExtractionResult schema from Apache PDFBox\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"documentId\": {\n      \"type\": \"string\",\n      \"example\": \"doc-abc123\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"example\": \"This is extracted text from the PDF document.\"\n    },\n    \"pageCount\": {\n      \"type\": \"integer\",\n      \"example\": 5\n    },\n    \"wordCount\": {\n      \"type\": \"integer\",\n      \"example\": 1234\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pdfbox/refs/heads/main/json-schema/apache-pdfbox-text-extraction-result-schema.json
tags:
- Document Processing
- Java
- PDF
- Text Extraction
- Apache
- Open Source
title: TextExtractionResult
---
