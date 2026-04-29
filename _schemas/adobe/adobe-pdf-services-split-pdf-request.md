---
description: ''
layout: schema
name: SplitPDFRequest
properties_list:
- description: The asset ID of the PDF to split.
  name: assetID
  type: string
- description: Options controlling how the PDF is split.
  name: splitOptions
  type: object
provider_name: Adobe
provider_slug: adobe
schema_file: json-schema/adobe-pdf-services-split-pdf-request-schema.json
slug: adobe-pdf-services-split-pdf-request
source_filename: adobe-pdf-services-split-pdf-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SplitPDFRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"The asset ID of the PDF to split.\"\n    },\n    \"splitOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Options controlling how the PDF is split.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/json-schema/adobe-pdf-services-split-pdf-request-schema.json
tags:
- Analytics
- Creative Cloud
- Digital Asset Management
- Document Services
- E-Commerce
- E-Signatures
- Experience Cloud
- Generative AI
- Marketing
- PDF
- Work Management
title: SplitPDFRequest
---
