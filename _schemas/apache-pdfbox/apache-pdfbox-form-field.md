---
description: FormField schema from Apache PDFBox
layout: schema
name: FormField
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: value
  type: string
- description: ''
  name: required
  type: boolean
provider_name: Apache PDFBox
provider_slug: apache-pdfbox
schema_file: json-schema/apache-pdfbox-form-field-schema.json
slug: apache-pdfbox-form-field
source_filename: apache-pdfbox-form-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pdfbox/refs/heads/main/json-schema/apache-pdfbox-form-field-schema.json\",\n  \"title\": \"FormField\",\n  \"description\": \"FormField schema from Apache PDFBox\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"firstName\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"PDTextField\",\n      \"enum\": [\n        \"PDTextField\",\n        \"PDCheckBox\",\n        \"PDRadioButton\",\n        \"PDComboBox\",\n        \"PDListBox\",\n        \"PDSignatureField\"\n      ]\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"example\": \"John\"\n    },\n    \"required\": {\n      \"type\": \"boolean\",\n      \"example\": false\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pdfbox/refs/heads/main/json-schema/apache-pdfbox-form-field-schema.json
tags:
- Document Processing
- Java
- PDF
- Text Extraction
- Apache
- Open Source
title: FormField
---
