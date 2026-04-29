---
description: ''
layout: schema
name: PDFPropertiesRequest
properties_list:
- description: The asset ID of the PDF to inspect.
  name: assetID
  type: string
- description: Whether to include page-level property details.
  name: includePageLevelProperties
  type: boolean
provider_name: Adobe
provider_slug: adobe
schema_file: json-schema/adobe-pdf-services-pdf-properties-request-schema.json
slug: adobe-pdf-services-pdf-properties-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PDFPropertiesRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"The asset ID of the PDF to inspect.\"\n    },\n    \"includePageLevelProperties\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to include page-level property details.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/json-schema/adobe-pdf-services-pdf-properties-request-schema.json
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
title: PDFPropertiesRequest
---
