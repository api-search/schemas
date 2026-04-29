---
description: Web scraping result
layout: schema
name: WebScrapingResponse
properties_list:
- description: Full HTML content of the page
  name: body
  type: string
- description: Final URL after redirects
  name: url
  type: string
- description: HTTP status code of the scraped page
  name: status_code
  type: integer
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/web-scraping-web-scraping-response-schema.json
slug: web-scraping-web-scraping-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/web-scraping-web-scraping-response-schema.json\",\n  \"title\": \"WebScrapingResponse\",\n  \"description\": \"Web scraping result\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"Full HTML content of the page\",\n      \"example\": \"<html><head><title>Example Domain</title></head><body>...</body></html>\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Final URL after redirects\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"status_code\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code of the scraped page\",\n      \"example\": 200\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/web-scraping-web-scraping-response-schema.json
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
title: WebScrapingResponse
---
