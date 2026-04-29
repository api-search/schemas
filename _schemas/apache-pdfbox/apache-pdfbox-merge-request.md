---
description: MergeRequest schema from Apache PDFBox
layout: schema
name: MergeRequest
properties_list:
- description: ''
  name: sourceDocumentIds
  type: array
- description: ''
  name: outputTitle
  type: string
provider_name: Apache PDFBox
provider_slug: apache-pdfbox
schema_file: json-schema/apache-pdfbox-merge-request-schema.json
slug: apache-pdfbox-merge-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pdfbox/refs/heads/main/json-schema/apache-pdfbox-merge-request-schema.json\",\n  \"title\": \"MergeRequest\",\n  \"description\": \"MergeRequest schema from Apache PDFBox\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceDocumentIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"doc-001\",\n        \"doc-002\"\n      ]\n    },\n    \"outputTitle\": {\n      \"type\": \"string\",\n      \"example\": \"Merged Document\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pdfbox/refs/heads/main/json-schema/apache-pdfbox-merge-request-schema.json
tags:
- Document Processing
- Java
- PDF
- Text Extraction
- Apache
- Open Source
title: MergeRequest
---
