---
description: DocumentMetadata schema from Apache PDFBox
layout: schema
name: DocumentMetadata
properties_list:
- description: ''
  name: title
  type: string
- description: ''
  name: author
  type: string
- description: ''
  name: subject
  type: string
- description: ''
  name: creator
  type: string
- description: ''
  name: producer
  type: string
- description: ''
  name: creationDate
  type: string
- description: ''
  name: modificationDate
  type: string
provider_name: Apache PDFBox
provider_slug: apache-pdfbox
schema_file: json-schema/apache-pdfbox-document-metadata-schema.json
slug: apache-pdfbox-document-metadata
source_filename: apache-pdfbox-document-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pdfbox/refs/heads/main/json-schema/apache-pdfbox-document-metadata-schema.json\",\n  \"title\": \"DocumentMetadata\",\n  \"description\": \"DocumentMetadata schema from Apache PDFBox\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"example\": \"Annual Report 2026\"\n    },\n    \"author\": {\n      \"type\": \"string\",\n      \"example\": \"Jane Doe\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"example\": \"Financial Summary\"\n    },\n    \"creator\": {\n      \"type\": \"string\",\n      \"example\": \"Apache PDFBox\"\n    },\n    \"producer\": {\n      \"type\": \"string\",\n      \"example\": \"Apache PDFBox\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-19T10:00:00Z\"\n    },\n\
  \    \"modificationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-19T11:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pdfbox/refs/heads/main/json-schema/apache-pdfbox-document-metadata-schema.json
tags:
- Document Processing
- Java
- PDF
- Text Extraction
- Apache
- Open Source
title: DocumentMetadata
---
