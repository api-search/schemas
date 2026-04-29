---
description: Error or rate limit response from Alpha Vantage
layout: schema
name: ErrorResponse
properties_list:
- description: API rate limit or usage note
  name: Note
  type: string
- description: Premium endpoint or invalid request information
  name: Information
  type: string
- description: Error message for invalid parameters
  name: Error Message
  type: string
provider_name: Alpha Vantage
provider_slug: alpha-vantage
schema_file: json-schema/alpha-vantage-error_response-schema.json
slug: alpha-vantage-error_response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.alphavantage.co/schemas/alpha-vantage-error_response-schema.json\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Error or rate limit response from Alpha Vantage\",\n  \"properties\": {\n    \"Note\": {\n      \"type\": \"string\",\n      \"description\": \"API rate limit or usage note\"\n    },\n    \"Information\": {\n      \"type\": \"string\",\n      \"description\": \"Premium endpoint or invalid request information\"\n    },\n    \"Error Message\": {\n      \"type\": \"string\",\n      \"description\": \"Error message for invalid parameters\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alpha-vantage/refs/heads/main/json-schema/alpha-vantage-error_response-schema.json
tags:
- Financial
- Market Data
- Stocks
- Technical Indicators
- Economic Data
- Sentiment Analysis
title: ErrorResponse
---
