---
description: ''
layout: schema
name: ReorderPagesRequest
properties_list:
- description: The asset ID of the PDF to reorder.
  name: assetID
  type: string
- description: The desired page order as an array of 1-based page numbers.
  name: pagesOrder
  type: array
provider_name: Adobe
provider_slug: adobe
schema_file: json-schema/adobe-pdf-services-reorder-pages-request-schema.json
slug: adobe-pdf-services-reorder-pages-request
source_filename: adobe-pdf-services-reorder-pages-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReorderPagesRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"The asset ID of the PDF to reorder.\"\n    },\n    \"pagesOrder\": {\n      \"type\": \"array\",\n      \"description\": \"The desired page order as an array of 1-based page numbers.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/json-schema/adobe-pdf-services-reorder-pages-request-schema.json
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
title: ReorderPagesRequest
---
