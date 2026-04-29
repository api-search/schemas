---
description: ''
layout: schema
name: AutoTagRequest
properties_list:
- description: The asset ID of the PDF to auto-tag.
  name: assetID
  type: string
- description: Whether to generate an accessibility tagging report.
  name: generateReport
  type: boolean
- description: Whether to shift heading levels to start at H1.
  name: shiftHeadings
  type: boolean
provider_name: Adobe
provider_slug: adobe
schema_file: json-schema/adobe-pdf-services-auto-tag-request-schema.json
slug: adobe-pdf-services-auto-tag-request
source_filename: adobe-pdf-services-auto-tag-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AutoTagRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"The asset ID of the PDF to auto-tag.\"\n    },\n    \"generateReport\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to generate an accessibility tagging report.\"\n    },\n    \"shiftHeadings\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to shift heading levels to start at H1.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/json-schema/adobe-pdf-services-auto-tag-request-schema.json
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
title: AutoTagRequest
---
