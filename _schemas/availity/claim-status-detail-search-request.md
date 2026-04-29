---
description: DetailSearchRequest schema from Availity API
layout: schema
name: DetailSearchRequest
properties_list:
- description: ''
  name: payerId
  type: string
- description: ''
  name: claimNumber
  type: string
- description: ''
  name: requestType
  type: string
- description: ''
  name: providerTaxId
  type: string
- description: ''
  name: providerNpi
  type: string
- description: ''
  name: processedDate
  type: string
provider_name: availity
provider_slug: availity
schema_file: json-schema/claim-status-detail-search-request-schema.json
slug: claim-status-detail-search-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/claim-status-detail-search-request-schema.json\",\n  \"title\": \"DetailSearchRequest\",\n  \"description\": \"DetailSearchRequest schema from Availity API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"payerId\",\n    \"claimNumber\",\n    \"requestType\"\n  ],\n  \"properties\": {\n    \"payerId\": {\n      \"type\": \"string\",\n      \"example\": \"BCBS001\"\n    },\n    \"claimNumber\": {\n      \"type\": \"string\",\n      \"example\": \"CLM-2025-001234\"\n    },\n    \"requestType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CLAIM_NUMBER\"\n      ],\n      \"example\": \"CLAIM_NUMBER\"\n    },\n    \"providerTaxId\": {\n      \"type\": \"string\",\n      \"example\": \"123456789\"\n    },\n    \"providerNpi\": {\n      \"type\": \"string\",\n      \"example\": \"1234567890\"\n\
  \    },\n    \"processedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"2025-03-15\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/claim-status-detail-search-request-schema.json
tags: []
title: DetailSearchRequest
---
