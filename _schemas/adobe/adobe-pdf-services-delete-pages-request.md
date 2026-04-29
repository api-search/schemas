---
description: ''
layout: schema
name: DeletePagesRequest
properties_list:
- description: The asset ID of the PDF from which to delete pages.
  name: assetID
  type: string
- description: Page ranges to delete.
  name: pageRanges
  type: array
provider_name: Adobe
provider_slug: adobe
schema_file: json-schema/adobe-pdf-services-delete-pages-request-schema.json
slug: adobe-pdf-services-delete-pages-request
source_filename: adobe-pdf-services-delete-pages-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeletePagesRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"The asset ID of the PDF from which to delete pages.\"\n    },\n    \"pageRanges\": {\n      \"type\": \"array\",\n      \"description\": \"Page ranges to delete.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/json-schema/adobe-pdf-services-delete-pages-request-schema.json
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
title: DeletePagesRequest
---
