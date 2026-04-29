---
description: ''
layout: schema
name: InsertPagesRequest
properties_list:
- description: The asset ID of the base PDF.
  name: baseAssetID
  type: string
- description: Assets and positions for insertion.
  name: assetsToInsert
  type: array
provider_name: Adobe
provider_slug: adobe
schema_file: json-schema/adobe-pdf-services-insert-pages-request-schema.json
slug: adobe-pdf-services-insert-pages-request
source_filename: adobe-pdf-services-insert-pages-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InsertPagesRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"baseAssetID\": {\n      \"type\": \"string\",\n      \"description\": \"The asset ID of the base PDF.\"\n    },\n    \"assetsToInsert\": {\n      \"type\": \"array\",\n      \"description\": \"Assets and positions for insertion.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/json-schema/adobe-pdf-services-insert-pages-request-schema.json
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
title: InsertPagesRequest
---
