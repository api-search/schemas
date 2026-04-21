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
tags:
- Financial
- Market Data
- Stocks
- Technical Indicators
- Economic Data
- Sentiment Analysis
title: ErrorResponse
---
