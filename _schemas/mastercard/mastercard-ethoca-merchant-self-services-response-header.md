---
description: ''
layout: schema
name: ResponseHeader
properties_list:
- description: Total number of records found
  name: totalRecords
  type: integer
- description: Total number of pages based on limit
  name: totalPages
  type: integer
- description: The current page number
  name: currentPage
  type: integer
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-response-header-schema.json
slug: mastercard-ethoca-merchant-self-services-response-header
source_filename: mastercard-ethoca-merchant-self-services-response-header-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResponseHeader\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalRecords\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of records found\"\n    },\n    \"totalPages\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of pages based on limit\"\n    },\n    \"currentPage\": {\n      \"type\": \"integer\",\n      \"description\": \"The current page number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-response-header-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: ResponseHeader
---
