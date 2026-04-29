---
description: TimezoneInfo schema from Abstract API ip-intelligence
layout: schema
name: TimezoneInfo
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: abbreviation
  type: string
- description: ''
  name: utc_offset
  type: integer
- description: ''
  name: local_time
  type: string
- description: ''
  name: is_dst
  type: boolean
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/ip-intelligence-timezone-info-schema.json
slug: ip-intelligence-timezone-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/ip-intelligence-timezone-info-schema.json\",\n  \"title\": \"TimezoneInfo\",\n  \"description\": \"TimezoneInfo schema from Abstract API ip-intelligence\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"America/Los_Angeles\"\n    },\n    \"abbreviation\": {\n      \"type\": \"string\",\n      \"example\": \"PST\"\n    },\n    \"utc_offset\": {\n      \"type\": \"integer\",\n      \"example\": -8\n    },\n    \"local_time\": {\n      \"type\": \"string\",\n      \"example\": \"2026-04-19T10:30:00\"\n    },\n    \"is_dst\": {\n      \"type\": \"boolean\",\n      \"example\": false\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/ip-intelligence-timezone-info-schema.json
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
title: TimezoneInfo
---
