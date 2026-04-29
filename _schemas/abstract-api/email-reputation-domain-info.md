---
description: Domain-level information
layout: schema
name: DomainInfo
properties_list:
- description: Domain extracted from email
  name: domain
  type: string
- description: Age of the domain in days
  name: domain_age
  type: integer
- description: Whether the domain hosts a live website
  name: is_live_site
  type: boolean
- description: Domain registrar name
  name: registrar
  type: string
- description: URL of the registrar
  name: registrar_url
  type: string
- description: Date the domain was registered
  name: date_registered
  type: string
- description: Date the domain was last renewed
  name: date_last_renewed
  type: string
- description: Date the domain expires
  name: date_expires
  type: string
- description: Whether the TLD is associated with risky domains
  name: is_risky_tld
  type: boolean
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/email-reputation-domain-info-schema.json
slug: email-reputation-domain-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/email-reputation-domain-info-schema.json\",\n  \"title\": \"DomainInfo\",\n  \"description\": \"Domain-level information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Domain extracted from email\",\n      \"example\": \"example.com\"\n    },\n    \"domain_age\": {\n      \"type\": \"integer\",\n      \"description\": \"Age of the domain in days\",\n      \"example\": 9000\n    },\n    \"is_live_site\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the domain hosts a live website\",\n      \"example\": true\n    },\n    \"registrar\": {\n      \"type\": \"string\",\n      \"description\": \"Domain registrar name\",\n      \"example\": \"GoDaddy\"\n    },\n    \"registrar_url\": {\n      \"type\": \"string\",\n\
  \      \"format\": \"uri\",\n      \"description\": \"URL of the registrar\",\n      \"example\": \"https://www.godaddy.com\"\n    },\n    \"date_registered\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the domain was registered\",\n      \"example\": \"2015-03-10\"\n    },\n    \"date_last_renewed\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the domain was last renewed\",\n      \"example\": \"2025-03-10\"\n    },\n    \"date_expires\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the domain expires\",\n      \"example\": \"2026-03-10\"\n    },\n    \"is_risky_tld\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the TLD is associated with risky domains\",\n      \"example\": false\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/email-reputation-domain-info-schema.json
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
title: DomainInfo
---
