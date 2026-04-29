---
description: Email deliverability information
layout: schema
name: Deliverability
properties_list:
- description: Overall deliverability status
  name: status
  type: string
- description: Detailed deliverability reason
  name: status_detail
  type: string
- description: Whether the email format is valid
  name: is_format_valid
  type: boolean
- description: Whether the SMTP server responded positively
  name: is_smtp_valid
  type: boolean
- description: Whether valid MX records exist for the domain
  name: is_mx_valid
  type: boolean
- description: List of MX records for the domain
  name: mx_records
  type: array
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/email-reputation-deliverability-schema.json
slug: email-reputation-deliverability
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/email-reputation-deliverability-schema.json\",\n  \"title\": \"Deliverability\",\n  \"description\": \"Email deliverability information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Overall deliverability status\",\n      \"example\": \"DELIVERABLE\",\n      \"enum\": [\n        \"DELIVERABLE\",\n        \"UNDELIVERABLE\",\n        \"RISKY\",\n        \"UNKNOWN\"\n      ]\n    },\n    \"status_detail\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed deliverability reason\",\n      \"example\": \"smtp_valid\"\n    },\n    \"is_format_valid\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the email format is valid\",\n      \"example\": true\n    },\n    \"is_smtp_valid\": {\n      \"type\": \"\
  boolean\",\n      \"description\": \"Whether the SMTP server responded positively\",\n      \"example\": true\n    },\n    \"is_mx_valid\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether valid MX records exist for the domain\",\n      \"example\": true\n    },\n    \"mx_records\": {\n      \"type\": \"array\",\n      \"description\": \"List of MX records for the domain\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"mx.example.com\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/email-reputation-deliverability-schema.json
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
title: Deliverability
---
