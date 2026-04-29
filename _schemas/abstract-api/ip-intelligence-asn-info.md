---
description: Autonomous System Number information
layout: schema
name: ASNInfo
properties_list:
- description: ASN identifier
  name: asn
  type: string
- description: ASN organization name
  name: name
  type: string
- description: Primary domain for the ASN
  name: domain
  type: string
- description: Type of ASN (hosting, isp, business, etc.)
  name: type
  type: string
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/ip-intelligence-asn-info-schema.json
slug: ip-intelligence-asn-info
source_filename: ip-intelligence-asn-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/ip-intelligence-asn-info-schema.json\",\n  \"title\": \"ASNInfo\",\n  \"description\": \"Autonomous System Number information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"asn\": {\n      \"type\": \"string\",\n      \"description\": \"ASN identifier\",\n      \"example\": \"AS15169\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"ASN organization name\",\n      \"example\": \"Google LLC\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Primary domain for the ASN\",\n      \"example\": \"google.com\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of ASN (hosting, isp, business, etc.)\",\n      \"example\": \"hosting\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/ip-intelligence-asn-info-schema.json
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
title: ASNInfo
---
