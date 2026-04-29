---
description: ''
layout: schema
name: GovernmentLookupRequest
properties_list:
- description: Country or ticker search string
  name: query
  type: string
- description: ''
  name: partialMatch
  type: boolean
- description: ''
  name: maxResults
  type: integer
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-http-government-lookup-request-schema.json
slug: bloomberg-http-government-lookup-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GovernmentLookupRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"Country or ticker search string\"\n    },\n    \"partialMatch\": {\n      \"type\": \"boolean\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-http-government-lookup-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: GovernmentLookupRequest
---
