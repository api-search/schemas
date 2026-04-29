---
description: Historical Identifier Resolution data object.
layout: schema
name: identifierResolutionHistorical
properties_list:
- description: Identifier inputted in the request.
  name: requestId
  type: string
- description: The type of identifier inputted in the request
  name: inputSymbolType
  type: string
- description: Name of the requested identifier
  name: name
  type: string
- description: The 3 digit fref exchange code for the primary exchange of the security
  name: frefListingExchange
  type: string
- description: The 3 digit ISO code for the currency
  name: currency
  type: string
- description: Type of identifier outputted.
  name: outputType
  type: string
- description: Requested identifier.
  name: value
  type: string
- description: Start Date in YYYY-MM-DD format.
  name: startDate
  type: string
- description: End Date in YYYY-MM-DD format.
  name: endDate
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-symbology-identifier-resolution-historical-schema.json
slug: factset-symbology-identifier-resolution-historical
source_filename: factset-symbology-identifier-resolution-historical-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"identifierResolutionHistorical\",\n  \"type\": \"object\",\n  \"description\": \"Historical Identifier Resolution data object.\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier inputted in the request.\"\n    },\n    \"inputSymbolType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of identifier inputted in the request\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the requested identifier\"\n    },\n    \"frefListingExchange\": {\n      \"type\": \"string\",\n      \"description\": \"The 3 digit fref exchange code for the primary exchange of the security\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"The 3 digit ISO code for the currency\"\n    },\n    \"outputType\": {\n      \"type\": \"string\",\n      \"description\": \"Type\
  \ of identifier outputted.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Requested identifier.\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"description\": \"Start Date in YYYY-MM-DD format.\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"description\": \"End Date in YYYY-MM-DD format.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-symbology-identifier-resolution-historical-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: identifierResolutionHistorical
---
