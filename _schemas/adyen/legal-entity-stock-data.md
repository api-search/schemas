---
description: StockData schema from Adyen API
layout: schema
name: StockData
properties_list:
- description: The four-digit [Market Identifier Code](https://en.wikipedia.org/wiki/Market_Identifier_Code) of the stock market where the organization's stocks are traded.
  name: marketIdentifier
  type: string
- description: The 12-digit International Securities Identification Number (ISIN) of the company, without dashes (-).
  name: stockNumber
  type: string
- description: The stock ticker symbol.
  name: tickerSymbol
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-stock-data-schema.json
slug: legal-entity-stock-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-stock-data-schema.json\",\n  \"title\": \"StockData\",\n  \"description\": \"StockData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"marketIdentifier\": {\n      \"description\": \"The four-digit [Market Identifier Code](https://en.wikipedia.org/wiki/Market_Identifier_Code) of the stock market where the organization's stocks are traded.\",\n      \"type\": \"string\"\n    },\n    \"stockNumber\": {\n      \"description\": \"The 12-digit International Securities Identification Number (ISIN) of the company, without dashes (-).\",\n      \"type\": \"string\"\n    },\n    \"tickerSymbol\": {\n      \"description\": \"The stock ticker symbol.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-stock-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: StockData
---
