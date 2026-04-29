---
description: ''
layout: schema
name: ExtractPDFRequest
properties_list:
- description: The asset ID of the PDF to extract from.
  name: assetID
  type: string
- description: The types of elements to extract from the PDF.
  name: elementsToExtract
  type: array
- description: Rendition types to generate for extracted elements.
  name: elementsToExtractRenditions
  type: array
- description: The output format for extracted tables.
  name: tableOutputFormat
  type: string
- description: Whether to include styling information (font, color, etc.) in the extraction output.
  name: getStylingInfo
  type: boolean
- description: Whether to include character-level bounding box information.
  name: addCharInfo
  type: boolean
provider_name: Adobe
provider_slug: adobe
schema_file: json-schema/adobe-pdf-services-extract-pdf-request-schema.json
slug: adobe-pdf-services-extract-pdf-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExtractPDFRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"The asset ID of the PDF to extract from.\"\n    },\n    \"elementsToExtract\": {\n      \"type\": \"array\",\n      \"description\": \"The types of elements to extract from the PDF.\"\n    },\n    \"elementsToExtractRenditions\": {\n      \"type\": \"array\",\n      \"description\": \"Rendition types to generate for extracted elements.\"\n    },\n    \"tableOutputFormat\": {\n      \"type\": \"string\",\n      \"description\": \"The output format for extracted tables.\"\n    },\n    \"getStylingInfo\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to include styling information (font, color, etc.) in the extraction output.\"\n    },\n    \"addCharInfo\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to include character-level\
  \ bounding box information.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/json-schema/adobe-pdf-services-extract-pdf-request-schema.json
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
title: ExtractPDFRequest
---
