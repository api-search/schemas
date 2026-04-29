---
description: ''
layout: schema
name: RotatePagesRequest
properties_list:
- description: The asset ID of the PDF containing pages to rotate.
  name: assetID
  type: string
- description: Rotation actions to apply to page ranges.
  name: pageActions
  type: array
provider_name: Adobe
provider_slug: adobe
schema_file: json-schema/adobe-pdf-services-rotate-pages-request-schema.json
slug: adobe-pdf-services-rotate-pages-request
source_filename: adobe-pdf-services-rotate-pages-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RotatePagesRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"The asset ID of the PDF containing pages to rotate.\"\n    },\n    \"pageActions\": {\n      \"type\": \"array\",\n      \"description\": \"Rotation actions to apply to page ranges.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/json-schema/adobe-pdf-services-rotate-pages-request-schema.json
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
title: RotatePagesRequest
---
