---
description: PageList schema from Apache PDFBox
layout: schema
name: PageList
properties_list:
- description: ''
  name: documentId
  type: string
- description: ''
  name: totalPages
  type: integer
- description: ''
  name: pages
  type: array
provider_name: Apache PDFBox
provider_slug: apache-pdfbox
schema_file: json-schema/apache-pdfbox-page-list-schema.json
slug: apache-pdfbox-page-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pdfbox/refs/heads/main/json-schema/apache-pdfbox-page-list-schema.json\",\n  \"title\": \"PageList\",\n  \"description\": \"PageList schema from Apache PDFBox\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"documentId\": {\n      \"type\": \"string\",\n      \"example\": \"doc-abc123\"\n    },\n    \"totalPages\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"pages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PageInfo\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pdfbox/refs/heads/main/json-schema/apache-pdfbox-page-list-schema.json
tags:
- Document Processing
- Java
- PDF
- Text Extraction
- Apache
- Open Source
title: PageList
---
