---
description: ''
layout: schema
name: DocumentGenerationRequest
properties_list:
- description: The asset ID of the Word template (DOCX).
  name: assetID
  type: string
- description: The JSON data to merge with the template.
  name: jsonDataForMerge
  type: object
- description: The desired output format.
  name: outputFormat
  type: string
- description: Reusable document fragments for template composition.
  name: fragments
  type: object
provider_name: Adobe
provider_slug: adobe
schema_file: json-schema/adobe-pdf-services-document-generation-request-schema.json
slug: adobe-pdf-services-document-generation-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DocumentGenerationRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"The asset ID of the Word template (DOCX).\"\n    },\n    \"jsonDataForMerge\": {\n      \"type\": \"object\",\n      \"description\": \"The JSON data to merge with the template.\"\n    },\n    \"outputFormat\": {\n      \"type\": \"string\",\n      \"description\": \"The desired output format.\"\n    },\n    \"fragments\": {\n      \"type\": \"object\",\n      \"description\": \"Reusable document fragments for template composition.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/json-schema/adobe-pdf-services-document-generation-request-schema.json
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
title: DocumentGenerationRequest
---
