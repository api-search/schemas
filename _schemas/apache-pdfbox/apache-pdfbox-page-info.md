---
description: PageInfo schema from Apache PDFBox
layout: schema
name: PageInfo
properties_list:
- description: ''
  name: pageNumber
  type: integer
- description: ''
  name: width
  type: number
- description: ''
  name: height
  type: number
- description: ''
  name: rotation
  type: integer
provider_name: Apache PDFBox
provider_slug: apache-pdfbox
schema_file: json-schema/apache-pdfbox-page-info-schema.json
slug: apache-pdfbox-page-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pdfbox/refs/heads/main/json-schema/apache-pdfbox-page-info-schema.json\",\n  \"title\": \"PageInfo\",\n  \"description\": \"PageInfo schema from Apache PDFBox\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pageNumber\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"width\": {\n      \"type\": \"number\",\n      \"example\": 595.0\n    },\n    \"height\": {\n      \"type\": \"number\",\n      \"example\": 842.0\n    },\n    \"rotation\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pdfbox/refs/heads/main/json-schema/apache-pdfbox-page-info-schema.json
tags:
- Document Processing
- Java
- PDF
- Text Extraction
- Apache
- Open Source
title: PageInfo
---
