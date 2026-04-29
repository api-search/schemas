---
description: Security reference data from Aladdin
layout: schema
name: Security
properties_list:
- description: Internal Aladdin security identifier
  name: securityId
  type: string
- description: Security full name
  name: name
  type: string
- description: Exchange ticker symbol
  name: ticker
  type: string
- description: ISIN identifier
  name: isin
  type: string
- description: CUSIP identifier
  name: cusip
  type: string
- description: Asset class classification
  name: assetClass
  type: string
- description: GICS sector
  name: sector
  type: string
- description: Country of domicile ISO code
  name: country
  type: string
- description: Trading currency ISO code
  name: currency
  type: string
- description: Primary exchange
  name: exchange
  type: string
provider_name: Aladdin Studio
provider_slug: aladdin-studio
schema_file: json-schema/aladdin-studio-graph-security-schema.json
slug: aladdin-studio-graph-security
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-graph-security-schema.json\",\n  \"title\": \"Security\",\n  \"description\": \"Security reference data from Aladdin\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"securityId\": {\n      \"type\": \"string\",\n      \"description\": \"Internal Aladdin security identifier\",\n      \"example\": \"US0378331005\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Security full name\",\n      \"example\": \"Apple Inc\"\n    },\n    \"ticker\": {\n      \"type\": \"string\",\n      \"description\": \"Exchange ticker symbol\",\n      \"example\": \"AAPL\"\n    },\n    \"isin\": {\n      \"type\": \"string\",\n      \"description\": \"ISIN identifier\",\n      \"example\": \"US0378331005\"\n    },\n    \"cusip\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"CUSIP identifier\",\n      \"example\": 37833100\n    },\n    \"assetClass\": {\n      \"type\": \"string\",\n      \"description\": \"Asset class classification\",\n      \"example\": \"Equity\"\n    },\n    \"sector\": {\n      \"type\": \"string\",\n      \"description\": \"GICS sector\",\n      \"example\": \"Technology\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country of domicile ISO code\",\n      \"example\": \"US\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Trading currency ISO code\",\n      \"example\": \"USD\"\n    },\n    \"exchange\": {\n      \"type\": \"string\",\n      \"description\": \"Primary exchange\",\n      \"example\": \"NASDAQ\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-graph-security-schema.json
tags:
- Financial
- Investment Management
- Portfolio Analytics
- Risk Management
- Asset Management
- BlackRock
- Data Cloud
title: Security
---
