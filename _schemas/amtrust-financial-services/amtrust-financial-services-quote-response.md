---
description: Quote response
layout: schema
name: QuoteResponse
properties_list:
- description: Unique quote identifier
  name: quote_id
  type: string
- description: Quote status
  name: status
  type: string
- description: Annual premium amount
  name: premium
  type: number
- description: Insurance product type
  name: product_type
  type: string
- description: Policy effective date
  name: effective_date
  type: string
- description: Policy expiration date
  name: expiration_date
  type: string
- description: ''
  name: insured
  type: object
- description: Whether this quote can be bound online
  name: bind_online
  type: boolean
- description: Quote creation timestamp
  name: created_at
  type: string
- description: Quote expiration timestamp
  name: expires_at
  type: string
provider_name: AmTrust Financial Services
provider_slug: amtrust-financial-services
schema_file: json-schema/amtrust-financial-services-quote-response-schema.json
slug: amtrust-financial-services-quote-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/json-schema/amtrust-financial-services-quote-response-schema.json\",\n  \"title\": \"QuoteResponse\",\n  \"description\": \"Quote response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"quote_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique quote identifier\",\n      \"example\": \"QT-2025-78901\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Quote status\",\n      \"enum\": [\n        \"pending\",\n        \"quoted\",\n        \"bound\",\n        \"expired\"\n      ],\n      \"example\": \"quoted\"\n    },\n    \"premium\": {\n      \"type\": \"number\",\n      \"description\": \"Annual premium amount\",\n      \"example\": 8250.0\n    },\n    \"product_type\": {\n      \"type\": \"string\",\n      \"description\": \"Insurance product type\"\
  ,\n      \"example\": \"workers_compensation\"\n    },\n    \"effective_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Policy effective date\",\n      \"example\": \"2025-07-01\"\n    },\n    \"expiration_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Policy expiration date\",\n      \"example\": \"2026-07-01\"\n    },\n    \"insured\": {\n      \"$ref\": \"#/components/schemas/Insured\"\n    },\n    \"bind_online\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this quote can be bound online\",\n      \"example\": true\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Quote creation timestamp\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"expires_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Quote expiration timestamp\",\n      \"example\"\
  : \"2025-04-14T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/json-schema/amtrust-financial-services-quote-response-schema.json
tags:
- Commercial Insurance
- Insurance
- Property And Casualty
- Small Business
- Workers Compensation
title: QuoteResponse
---
