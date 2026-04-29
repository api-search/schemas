---
description: Image processing result
layout: schema
name: ImageProcessingResponse
properties_list:
- description: Original file size in bytes
  name: original_size
  type: integer
- description: Processed file size in bytes
  name: new_size
  type: integer
- description: Bytes saved by processing
  name: saved_bytes
  type: integer
- description: Percentage of size reduction
  name: saved_percent
  type: number
- description: URL to download the processed image
  name: url
  type: string
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/image-processing-image-processing-response-schema.json
slug: image-processing-image-processing-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/image-processing-image-processing-response-schema.json\",\n  \"title\": \"ImageProcessingResponse\",\n  \"description\": \"Image processing result\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"original_size\": {\n      \"type\": \"integer\",\n      \"description\": \"Original file size in bytes\",\n      \"example\": 102400\n    },\n    \"new_size\": {\n      \"type\": \"integer\",\n      \"description\": \"Processed file size in bytes\",\n      \"example\": 51200\n    },\n    \"saved_bytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Bytes saved by processing\",\n      \"example\": 51200\n    },\n    \"saved_percent\": {\n      \"type\": \"number\",\n      \"description\": \"Percentage of size reduction\",\n      \"example\": 50.0\n    },\n    \"url\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"uri\",\n      \"description\": \"URL to download the processed image\",\n      \"example\": \"https://dl.abstractapi.com/processed/abc123.webp\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/image-processing-image-processing-response-schema.json
tags:
- Avatars
- Company Enrichment
- Contacts
- Currencies
- Email Validation
- Exchange Rates
- IBAN Validation
- Image Processing
- IP Geolocation
- IP Intelligence
- Phone Validation
- Public Holidays
- Screenshots
- Timezones
- VAT Validation
- Web Scraping
title: ImageProcessingResponse
---
