---
description: TimezoneInfo schema from Abstract API ip-geolocation
layout: schema
name: TimezoneInfo
properties_list:
- description: IANA timezone name
  name: name
  type: string
- description: Timezone abbreviation
  name: abbreviation
  type: string
- description: GMT/UTC offset in hours
  name: gmt_offset
  type: integer
- description: Current local time
  name: current_time
  type: string
- description: Whether daylight saving time is active
  name: is_dst
  type: boolean
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/ip-geolocation-timezone-info-schema.json
slug: ip-geolocation-timezone-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/ip-geolocation-timezone-info-schema.json\",\n  \"title\": \"TimezoneInfo\",\n  \"description\": \"TimezoneInfo schema from Abstract API ip-geolocation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"IANA timezone name\",\n      \"example\": \"America/Los_Angeles\"\n    },\n    \"abbreviation\": {\n      \"type\": \"string\",\n      \"description\": \"Timezone abbreviation\",\n      \"example\": \"PST\"\n    },\n    \"gmt_offset\": {\n      \"type\": \"integer\",\n      \"description\": \"GMT/UTC offset in hours\",\n      \"example\": -8\n    },\n    \"current_time\": {\n      \"type\": \"string\",\n      \"description\": \"Current local time\",\n      \"example\": \"2026-04-19 10:30:00\"\n    },\n    \"is_dst\": {\n      \"type\": \"\
  boolean\",\n      \"description\": \"Whether daylight saving time is active\",\n      \"example\": false\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/ip-geolocation-timezone-info-schema.json
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
