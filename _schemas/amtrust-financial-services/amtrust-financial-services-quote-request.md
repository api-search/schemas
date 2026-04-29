---
description: Request to create a commercial lines quote
layout: schema
name: QuoteRequest
properties_list:
- description: Insurance product type
  name: product_type
  type: string
- description: US state abbreviation
  name: state
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
- description: Requested coverage details
  name: coverages
  type: array
- description: AmTrust agent identifier
  name: agent_id
  type: string
provider_name: AmTrust Financial Services
provider_slug: amtrust-financial-services
schema_file: json-schema/amtrust-financial-services-quote-request-schema.json
slug: amtrust-financial-services-quote-request
source_filename: amtrust-financial-services-quote-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/json-schema/amtrust-financial-services-quote-request-schema.json\",\n  \"title\": \"QuoteRequest\",\n  \"description\": \"Request to create a commercial lines quote\",\n  \"type\": \"object\",\n  \"required\": [\n    \"product_type\",\n    \"state\",\n    \"effective_date\",\n    \"insured\"\n  ],\n  \"properties\": {\n    \"product_type\": {\n      \"type\": \"string\",\n      \"description\": \"Insurance product type\",\n      \"enum\": [\n        \"workers_compensation\",\n        \"bop\",\n        \"general_liability\",\n        \"commercial_package\"\n      ]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"US state abbreviation\",\n      \"example\": \"TX\"\n    },\n    \"effective_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\"\
  : \"Policy effective date\",\n      \"example\": \"2025-07-01\"\n    },\n    \"expiration_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Policy expiration date\",\n      \"example\": \"2026-07-01\"\n    },\n    \"insured\": {\n      \"$ref\": \"#/components/schemas/Insured\"\n    },\n    \"coverages\": {\n      \"type\": \"array\",\n      \"description\": \"Requested coverage details\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Coverage\"\n      }\n    },\n    \"agent_id\": {\n      \"type\": \"string\",\n      \"description\": \"AmTrust agent identifier\",\n      \"example\": \"AGT-12345\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/json-schema/amtrust-financial-services-quote-request-schema.json
tags:
- Commercial Insurance
- Insurance
- Property And Casualty
- Small Business
- Workers Compensation
title: QuoteRequest
---
