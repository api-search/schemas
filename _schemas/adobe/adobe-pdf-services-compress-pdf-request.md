---
description: ''
layout: schema
name: CompressPDFRequest
properties_list:
- description: The asset ID of the PDF to compress.
  name: assetID
  type: string
- description: The desired compression level. Higher compression results in smaller files but may reduce image quality.
  name: compressionLevel
  type: string
provider_name: Adobe
provider_slug: adobe
schema_file: json-schema/adobe-pdf-services-compress-pdf-request-schema.json
slug: adobe-pdf-services-compress-pdf-request
source_filename: adobe-pdf-services-compress-pdf-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompressPDFRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"The asset ID of the PDF to compress.\"\n    },\n    \"compressionLevel\": {\n      \"type\": \"string\",\n      \"description\": \"The desired compression level. Higher compression results in smaller files but may reduce image quality.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/json-schema/adobe-pdf-services-compress-pdf-request-schema.json
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
title: CompressPDFRequest
---
