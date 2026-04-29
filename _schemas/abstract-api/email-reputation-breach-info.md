---
description: Data breach history for the email
layout: schema
name: BreachInfo
properties_list:
- description: Total number of breaches the email appeared in
  name: total_breaches
  type: integer
- description: Date of the earliest known breach
  name: date_first_breached
  type: string
- description: Date of the most recent breach
  name: date_last_breached
  type: string
- description: Domains where the email was breached
  name: breached_domains
  type: array
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/email-reputation-breach-info-schema.json
slug: email-reputation-breach-info
source_filename: email-reputation-breach-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/email-reputation-breach-info-schema.json\",\n  \"title\": \"BreachInfo\",\n  \"description\": \"Data breach history for the email\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total_breaches\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of breaches the email appeared in\",\n      \"example\": 0\n    },\n    \"date_first_breached\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of the earliest known breach\",\n      \"example\": \"2020-01-15\"\n    },\n    \"date_last_breached\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of the most recent breach\",\n      \"example\": \"2023-06-01\"\n    },\n    \"breached_domains\": {\n      \"type\": \"array\",\n      \"description\": \"Domains\
  \ where the email was breached\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"breached-site.com\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/email-reputation-breach-info-schema.json
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
title: BreachInfo
---
