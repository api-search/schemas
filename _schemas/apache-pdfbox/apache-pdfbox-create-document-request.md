---
description: CreateDocumentRequest schema from Apache PDFBox
layout: schema
name: CreateDocumentRequest
properties_list:
- description: ''
  name: title
  type: string
- description: ''
  name: author
  type: string
- description: ''
  name: pageSize
  type: string
provider_name: Apache PDFBox
provider_slug: apache-pdfbox
schema_file: json-schema/apache-pdfbox-create-document-request-schema.json
slug: apache-pdfbox-create-document-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pdfbox/refs/heads/main/json-schema/apache-pdfbox-create-document-request-schema.json\",\n  \"title\": \"CreateDocumentRequest\",\n  \"description\": \"CreateDocumentRequest schema from Apache PDFBox\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"example\": \"My Document\"\n    },\n    \"author\": {\n      \"type\": \"string\",\n      \"example\": \"John Smith\"\n    },\n    \"pageSize\": {\n      \"type\": \"string\",\n      \"example\": \"A4\",\n      \"enum\": [\n        \"A4\",\n        \"LETTER\",\n        \"LEGAL\",\n        \"A3\",\n        \"A5\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pdfbox/refs/heads/main/json-schema/apache-pdfbox-create-document-request-schema.json
tags:
- Document Processing
- Java
- PDF
- Text Extraction
- Apache
- Open Source
title: CreateDocumentRequest
---
