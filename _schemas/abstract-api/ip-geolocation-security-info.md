---
description: SecurityInfo schema from Abstract API ip-geolocation
layout: schema
name: SecurityInfo
properties_list:
- description: Whether the IP is a known VPN
  name: is_vpn
  type: boolean
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/ip-geolocation-security-info-schema.json
slug: ip-geolocation-security-info
source_filename: ip-geolocation-security-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/ip-geolocation-security-info-schema.json\",\n  \"title\": \"SecurityInfo\",\n  \"description\": \"SecurityInfo schema from Abstract API ip-geolocation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"is_vpn\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the IP is a known VPN\",\n      \"example\": false\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/ip-geolocation-security-info-schema.json
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
title: SecurityInfo
---
