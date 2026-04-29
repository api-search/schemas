---
description: UltimateParentCompanyBusinessDetails schema from Adyen API
layout: schema
name: UltimateParentCompanyBusinessDetails
properties_list:
- description: The legal name of the company.
  name: legalBusinessName
  type: string
- description: The registration number of the company.
  name: registrationNumber
  type: string
- description: Market Identifier Code (MIC).
  name: stockExchange
  type: string
- description: International Securities Identification Number (ISIN).
  name: stockNumber
  type: string
- description: Stock Ticker symbol.
  name: stockTicker
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-ultimate-parent-company-business-details-schema.json
slug: notifications-ultimate-parent-company-business-details
source_filename: notifications-ultimate-parent-company-business-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-ultimate-parent-company-business-details-schema.json\",\n  \"title\": \"UltimateParentCompanyBusinessDetails\",\n  \"description\": \"UltimateParentCompanyBusinessDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"legalBusinessName\": {\n      \"description\": \"The legal name of the company.\",\n      \"type\": \"string\"\n    },\n    \"registrationNumber\": {\n      \"description\": \"The registration number of the company.\",\n      \"type\": \"string\"\n    },\n    \"stockExchange\": {\n      \"description\": \"Market Identifier Code (MIC).\",\n      \"type\": \"string\"\n    },\n    \"stockNumber\": {\n      \"description\": \"International Securities Identification Number (ISIN).\",\n      \"type\": \"string\"\n    },\n    \"stockTicker\": {\n      \"description\"\
  : \"Stock Ticker symbol.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-ultimate-parent-company-business-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UltimateParentCompanyBusinessDetails
---
