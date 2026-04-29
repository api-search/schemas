---
description: SignRequest schema from Apache PDFBox
layout: schema
name: SignRequest
properties_list:
- description: ''
  name: keystorePath
  type: string
- description: ''
  name: password
  type: string
- description: ''
  name: reason
  type: string
- description: ''
  name: location
  type: string
provider_name: Apache PDFBox
provider_slug: apache-pdfbox
schema_file: json-schema/apache-pdfbox-sign-request-schema.json
slug: apache-pdfbox-sign-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pdfbox/refs/heads/main/json-schema/apache-pdfbox-sign-request-schema.json\",\n  \"title\": \"SignRequest\",\n  \"description\": \"SignRequest schema from Apache PDFBox\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"keystorePath\": {\n      \"type\": \"string\",\n      \"example\": \"keystore.p12\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"example\": \"keystore-password\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"example\": \"Document approval\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"example\": \"San Francisco, CA\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pdfbox/refs/heads/main/json-schema/apache-pdfbox-sign-request-schema.json
tags:
- Document Processing
- Java
- PDF
- Text Extraction
- Apache
- Open Source
title: SignRequest
---
