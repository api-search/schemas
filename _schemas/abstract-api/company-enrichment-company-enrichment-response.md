---
description: Company enrichment data
layout: schema
name: CompanyEnrichmentResponse
properties_list:
- description: Company name
  name: name
  type: string
- description: Company domain
  name: domain
  type: string
- description: ISO 3166-1 alpha-2 country code
  name: country
  type: string
- description: City or locality
  name: locality
  type: string
- description: State or region
  name: region
  type: string
- description: LinkedIn company profile URL
  name: linkedin_url
  type: string
- description: URL to company logo image
  name: logo
  type: string
- description: Year the company was founded
  name: year_founded
  type: integer
- description: Industry classification
  name: industry
  type: string
- description: Approximate number of employees
  name: employees_count
  type: integer
- description: Short company description
  name: description
  type: string
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/company-enrichment-company-enrichment-response-schema.json
slug: company-enrichment-company-enrichment-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/company-enrichment-company-enrichment-response-schema.json\",\n  \"title\": \"CompanyEnrichmentResponse\",\n  \"description\": \"Company enrichment data\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Company name\",\n      \"example\": \"Stripe\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Company domain\",\n      \"example\": \"stripe.com\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code\",\n      \"example\": \"US\"\n    },\n    \"locality\": {\n      \"type\": \"string\",\n      \"description\": \"City or locality\",\n      \"example\": \"San Francisco\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"State or region\",\n      \"example\": \"California\"\n    },\n    \"linkedin_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"LinkedIn company profile URL\",\n      \"example\": \"https://www.linkedin.com/company/stripe\"\n    },\n    \"logo\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to company logo image\",\n      \"example\": \"https://logo.clearbit.com/stripe.com\"\n    },\n    \"year_founded\": {\n      \"type\": \"integer\",\n      \"description\": \"Year the company was founded\",\n      \"example\": 2010\n    },\n    \"industry\": {\n      \"type\": \"string\",\n      \"description\": \"Industry classification\",\n      \"example\": \"Financial Services\"\n    },\n    \"employees_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Approximate number of employees\",\n      \"example\": 8000\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Short company description\",\n      \"example\": \"Stripe is a technology company that builds economic infrastructure for the internet.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/company-enrichment-company-enrichment-response-schema.json
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
title: CompanyEnrichmentResponse
---
