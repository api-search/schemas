---
description: Time zone conversion result
layout: schema
name: ConvertTimeResponse
properties_list:
- description: Source location
  name: base_location
  type: string
- description: Input date and time
  name: base_datetime
  type: string
- description: Source IANA timezone name
  name: base_timezone_name
  type: string
- description: Source timezone abbreviation
  name: base_timezone_abbreviation
  type: string
- description: Source UTC offset in hours
  name: base_utc_offset
  type: integer
- description: Target location
  name: target_location
  type: string
- description: Converted date and time
  name: target_datetime
  type: string
- description: Target IANA timezone name
  name: target_timezone_name
  type: string
- description: Target timezone abbreviation
  name: target_timezone_abbreviation
  type: string
- description: Target UTC offset in hours
  name: target_utc_offset
  type: integer
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/timezones-convert-time-response-schema.json
slug: timezones-convert-time-response
source_filename: timezones-convert-time-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/timezones-convert-time-response-schema.json\",\n  \"title\": \"ConvertTimeResponse\",\n  \"description\": \"Time zone conversion result\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"base_location\": {\n      \"type\": \"string\",\n      \"description\": \"Source location\",\n      \"example\": \"London\"\n    },\n    \"base_datetime\": {\n      \"type\": \"string\",\n      \"description\": \"Input date and time\",\n      \"example\": \"2026-04-19 10:30:00\"\n    },\n    \"base_timezone_name\": {\n      \"type\": \"string\",\n      \"description\": \"Source IANA timezone name\",\n      \"example\": \"Europe/London\"\n    },\n    \"base_timezone_abbreviation\": {\n      \"type\": \"string\",\n      \"description\": \"Source timezone abbreviation\",\n      \"example\": \"BST\"\n    },\n    \"base_utc_offset\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Source UTC offset in hours\",\n      \"example\": 1\n    },\n    \"target_location\": {\n      \"type\": \"string\",\n      \"description\": \"Target location\",\n      \"example\": \"Tokyo\"\n    },\n    \"target_datetime\": {\n      \"type\": \"string\",\n      \"description\": \"Converted date and time\",\n      \"example\": \"2026-04-19 18:30:00\"\n    },\n    \"target_timezone_name\": {\n      \"type\": \"string\",\n      \"description\": \"Target IANA timezone name\",\n      \"example\": \"Asia/Tokyo\"\n    },\n    \"target_timezone_abbreviation\": {\n      \"type\": \"string\",\n      \"description\": \"Target timezone abbreviation\",\n      \"example\": \"JST\"\n    },\n    \"target_utc_offset\": {\n      \"type\": \"integer\",\n      \"description\": \"Target UTC offset in hours\",\n      \"example\": 9\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/timezones-convert-time-response-schema.json
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
title: ConvertTimeResponse
---
