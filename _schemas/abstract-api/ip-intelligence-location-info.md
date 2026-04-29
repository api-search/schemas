---
description: Geographic location for the IP
layout: schema
name: LocationInfo
properties_list:
- description: City name
  name: city
  type: string
- description: Region or state
  name: region
  type: string
- description: Country name
  name: country
  type: string
- description: ISO 3166-1 alpha-2 country code
  name: country_code
  type: string
- description: Latitude
  name: latitude
  type: number
- description: Longitude
  name: longitude
  type: number
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/ip-intelligence-location-info-schema.json
slug: ip-intelligence-location-info
source_filename: ip-intelligence-location-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/ip-intelligence-location-info-schema.json\",\n  \"title\": \"LocationInfo\",\n  \"description\": \"Geographic location for the IP\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City name\",\n      \"example\": \"Mountain View\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Region or state\",\n      \"example\": \"California\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country name\",\n      \"example\": \"United States\"\n    },\n    \"country_code\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code\",\n      \"example\": \"US\"\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n\
  \      \"description\": \"Latitude\",\n      \"example\": 37.386\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Longitude\",\n      \"example\": -122.0838\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/ip-intelligence-location-info-schema.json
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
title: LocationInfo
---
