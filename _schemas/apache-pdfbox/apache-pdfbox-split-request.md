---
description: SplitRequest schema from Apache PDFBox
layout: schema
name: SplitRequest
properties_list:
- description: Page numbers at which to split
  name: splitAtPages
  type: array
provider_name: Apache PDFBox
provider_slug: apache-pdfbox
schema_file: json-schema/apache-pdfbox-split-request-schema.json
slug: apache-pdfbox-split-request
source_filename: apache-pdfbox-split-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pdfbox/refs/heads/main/json-schema/apache-pdfbox-split-request-schema.json\",\n  \"title\": \"SplitRequest\",\n  \"description\": \"SplitRequest schema from Apache PDFBox\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"splitAtPages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"description\": \"Page numbers at which to split\",\n      \"example\": [\n        5,\n        10\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pdfbox/refs/heads/main/json-schema/apache-pdfbox-split-request-schema.json
tags:
- Document Processing
- Java
- PDF
- Text Extraction
- Apache
- Open Source
title: SplitRequest
---
