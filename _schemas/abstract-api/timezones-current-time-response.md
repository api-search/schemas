---
description: Current time and timezone data for a location
layout: schema
name: CurrentTimeResponse
properties_list:
- description: Current date and time in the target timezone
  name: datetime
  type: string
- description: IANA timezone name
  name: timezone_name
  type: string
- description: Human-readable location description
  name: timezone_location
  type: string
- description: Timezone abbreviation
  name: timezone_abbreviation
  type: string
- description: GMT/UTC offset in hours
  name: gmt_offset
  type: integer
- description: Whether daylight saving time is active
  name: is_dst
  type: boolean
- description: The input location string
  name: requested_location
  type: string
- description: Latitude of the location
  name: latitude
  type: number
- description: Longitude of the location
  name: longitude
  type: number
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/timezones-current-time-response-schema.json
slug: timezones-current-time-response
source_filename: timezones-current-time-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/timezones-current-time-response-schema.json\",\n  \"title\": \"CurrentTimeResponse\",\n  \"description\": \"Current time and timezone data for a location\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"datetime\": {\n      \"type\": \"string\",\n      \"description\": \"Current date and time in the target timezone\",\n      \"example\": \"2026-04-19 10:30:00\"\n    },\n    \"timezone_name\": {\n      \"type\": \"string\",\n      \"description\": \"IANA timezone name\",\n      \"example\": \"America/New_York\"\n    },\n    \"timezone_location\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable location description\",\n      \"example\": \"New York, United States\"\n    },\n    \"timezone_abbreviation\": {\n      \"type\": \"string\",\n      \"description\": \"Timezone abbreviation\"\
  ,\n      \"example\": \"EDT\"\n    },\n    \"gmt_offset\": {\n      \"type\": \"integer\",\n      \"description\": \"GMT/UTC offset in hours\",\n      \"example\": -4\n    },\n    \"is_dst\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether daylight saving time is active\",\n      \"example\": true\n    },\n    \"requested_location\": {\n      \"type\": \"string\",\n      \"description\": \"The input location string\",\n      \"example\": \"New York City\"\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Latitude of the location\",\n      \"example\": 40.7128\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Longitude of the location\",\n      \"example\": -74.006\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/timezones-current-time-response-schema.json
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
title: CurrentTimeResponse
---
