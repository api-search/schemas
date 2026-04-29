---
description: BusinessDetails schema from Adyen API
layout: schema
name: BusinessDetails
properties_list:
- description: The registered name of the company (if it differs from the legal name of the company).
  name: doingBusinessAs
  type: string
- description: The legal name of the company.
  name: legalBusinessName
  type: string
- description: Information about the parent public company. Required if the account holder is 100% owned by a publicly listed company.
  name: listedUltimateParentCompany
  type: array
- description: The registration number of the company.
  name: registrationNumber
  type: string
- description: Array containing information about individuals associated with the account holder either through ownership or control. For details about how you can identify them, refer to [our verification guide](ht
  name: shareholders
  type: array
- description: Signatories associated with the company. Each array entry should represent one signatory.
  name: signatories
  type: array
- description: Market Identifier Code (MIC).
  name: stockExchange
  type: string
- description: International Securities Identification Number (ISIN).
  name: stockNumber
  type: string
- description: Stock Ticker symbol.
  name: stockTicker
  type: string
- description: The tax ID of the company.
  name: taxId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-business-details-schema.json
slug: accounts-business-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-business-details-schema.json\",\n  \"title\": \"BusinessDetails\",\n  \"description\": \"BusinessDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"doingBusinessAs\": {\n      \"description\": \"The registered name of the company (if it differs from the legal name of the company).\",\n      \"type\": \"string\"\n    },\n    \"legalBusinessName\": {\n      \"description\": \"The legal name of the company.\",\n      \"type\": \"string\"\n    },\n    \"listedUltimateParentCompany\": {\n      \"description\": \"Information about the parent public company. Required if the account holder is 100% owned by a publicly listed company.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UltimateParentCompany\"\n      },\n      \"type\": \"array\"\n    },\n    \"registrationNumber\"\
  : {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The registration number of the company.\",\n      \"type\": \"string\"\n    },\n    \"shareholders\": {\n      \"description\": \"Array containing information about individuals associated with the account holder either through ownership or control. For details about how you can identify them, refer to [our verification guide](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process#identify-ubos).\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ShareholderContact\"\n      },\n      \"type\": \"array\"\n    },\n    \"signatories\": {\n      \"description\": \"Signatories associated with the company.\\nEach array entry should represent one signatory.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SignatoryContact\"\n      },\n      \"type\": \"array\"\n    },\n    \"stockExchange\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"Market Identifier Code\
  \ (MIC).\",\n      \"type\": \"string\"\n    },\n    \"stockNumber\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"International Securities Identification Number (ISIN).\",\n      \"type\": \"string\"\n    },\n    \"stockTicker\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"Stock Ticker symbol.\",\n      \"type\": \"string\"\n    },\n    \"taxId\": {\n      \"description\": \"The tax ID of the company.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-business-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BusinessDetails
---
