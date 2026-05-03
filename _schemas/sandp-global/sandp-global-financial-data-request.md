---
description: Schema for requesting financial and market intelligence data from the S&P Capital IQ API.
layout: schema
name: S&P Capital IQ Financial Data Request
properties_list:
- description: Array of data retrieval requests
  name: inputRequests
  type: array
provider_name: S&P Global
provider_slug: sandp-global
schema_file: json-schema/sandp-global-financial-data-request-schema.json
slug: sandp-global-financial-data-request
source_filename: sandp-global-financial-data-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/sandp-global/json-schema/financial-data-request.json\",\n  \"title\": \"S&P Capital IQ Financial Data Request\",\n  \"description\": \"Schema for requesting financial and market intelligence data from the S&P Capital IQ API.\",\n  \"type\": \"object\",\n  \"required\": [\"inputRequests\"],\n  \"properties\": {\n    \"inputRequests\": {\n      \"type\": \"array\",\n      \"description\": \"Array of data retrieval requests\",\n      \"minItems\": 1,\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"function\", \"identifier\", \"mnemonic\"],\n        \"properties\": {\n          \"function\": {\n            \"type\": \"string\",\n            \"description\": \"Data retrieval function code\",\n            \"enum\": [\"GDSP\", \"GDST\", \"GDSHE\", \"GDSHV\", \"GDSO\", \"GDSFIN\"],\n            \"examples\": [\"GDSP\"]\n          },\n     \
  \     \"identifier\": {\n            \"type\": \"string\",\n            \"description\": \"Company or security identifier (GVKEY, ticker, CUSIP, ISIN)\",\n            \"examples\": [\"IQ303931\", \"AAPL\", \"037833100\"]\n          },\n          \"mnemonic\": {\n            \"type\": \"string\",\n            \"description\": \"Data point mnemonic code for the specific financial metric\",\n            \"examples\": [\"IQ_TOTAL_REV\", \"IQ_NET_INC\", \"IQ_TOTAL_ASSETS\"]\n          },\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"Optional request properties for filtering and date ranges\",\n            \"properties\": {\n              \"startDate\": {\n                \"type\": \"string\",\n                \"format\": \"date\",\n                \"description\": \"Start date for time series (YYYY-MM-DD)\"\n              },\n              \"endDate\": {\n                \"type\": \"string\",\n                \"format\": \"date\",\n        \
  \        \"description\": \"End date for time series (YYYY-MM-DD)\"\n              },\n              \"periodType\": {\n                \"type\": \"string\",\n                \"enum\": [\"Annual\", \"Quarterly\", \"LTM\", \"YTD\", \"Semi-Annual\"],\n                \"description\": \"Financial period type\"\n              },\n              \"currency\": {\n                \"type\": \"string\",\n                \"pattern\": \"^[A-Z]{3}$\",\n                \"description\": \"Currency for financial data conversion\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sandp-global/refs/heads/main/json-schema/sandp-global-financial-data-request-schema.json
tags:
- Financial Data
- Market Intelligence
- Commodity Insights
- Credit Ratings
- Analytics
- Fortune 500
- Enterprise
title: S&P Capital IQ Financial Data Request
---
