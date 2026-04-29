---
description: FlagInfo schema from Abstract API ip-geolocation
layout: schema
name: FlagInfo
properties_list:
- description: Flag emoji
  name: emoji
  type: string
- description: Unicode code points for the flag
  name: unicode
  type: string
- description: URL to PNG flag image
  name: png
  type: string
- description: URL to SVG flag image
  name: svg
  type: string
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/ip-geolocation-flag-info-schema.json
slug: ip-geolocation-flag-info
source_filename: ip-geolocation-flag-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/ip-geolocation-flag-info-schema.json\",\n  \"title\": \"FlagInfo\",\n  \"description\": \"FlagInfo schema from Abstract API ip-geolocation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"emoji\": {\n      \"type\": \"string\",\n      \"description\": \"Flag emoji\",\n      \"example\": \"\\ud83c\\uddfa\\ud83c\\uddf8\"\n    },\n    \"unicode\": {\n      \"type\": \"string\",\n      \"description\": \"Unicode code points for the flag\",\n      \"example\": \"U+1F1FA U+1F1F8\"\n    },\n    \"png\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to PNG flag image\",\n      \"example\": \"https://static.abstractapi.com/country-flags/US_flag.png\"\n    },\n    \"svg\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to SVG\
  \ flag image\",\n      \"example\": \"https://static.abstractapi.com/country-flags/US_flag.svg\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/ip-geolocation-flag-info-schema.json
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
title: FlagInfo
---
