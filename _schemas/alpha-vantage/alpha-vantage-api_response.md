---
description: Generic Alpha Vantage API response containing Meta Data and time series or indicator data
layout: schema
name: ApiResponse
properties_list:
- description: Metadata about the response including symbol, indicator, and refresh timestamps
  name: Meta Data
  type: object
provider_name: Alpha Vantage
provider_slug: alpha-vantage
schema_file: json-schema/alpha-vantage-api_response-schema.json
slug: alpha-vantage-api_response
source_filename: alpha-vantage-api_response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.alphavantage.co/schemas/alpha-vantage-api_response-schema.json\",\n  \"title\": \"ApiResponse\",\n  \"type\": \"object\",\n  \"description\": \"Generic Alpha Vantage API response containing Meta Data and time series or indicator data\",\n  \"properties\": {\n    \"Meta Data\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata about the response including symbol, indicator, and refresh timestamps\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alpha-vantage/refs/heads/main/json-schema/alpha-vantage-api_response-schema.json
tags:
- Financial
- Market Data
- Stocks
- Technical Indicators
- Economic Data
- Sentiment Analysis
title: ApiResponse
---
