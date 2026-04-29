---
description: ''
layout: schema
name: sfdrPai
properties_list:
- description: FactSet Entity Identifier. Six alpha-numeric characters, excluding vowels, with a -E suffix (XXXXXX-E).
  name: fsymId
  type: string
- description: Identifier that was used for the request.
  name: requestId
  type: string
- description: Codes for the General, Mandatory and Additional PAI indicators
  name: subTopicCode
  type: string
- description: Names for the General, Mandatory and Additional PAI indicators
  name: subTopicName
  type: string
- description: The type of indicator - General, Additional & Mandatory
  name: indicatorType
  type: string
- description: The Reporting period end date expressed in YYYY-MM-DD format
  name: periodEndDate
  type: string
- description: The reporting period of the company expressed in YYYY format
  name: reportingPeriod
  type: string
- description: The units of measurements for the indicators
  name: standardizedUnit
  type: string
- description: The PAI calculations based on the company-reported data, some metrics sourced from Factset Databases and Truvalue SASB Spotlights
  name: standardizedValue
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-esg-sfdr-pai-schema.json
slug: factset-esg-sfdr-pai
source_filename: factset-esg-sfdr-pai-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"sfdrPai\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Entity Identifier. Six alpha-numeric characters, excluding vowels, with a -E suffix (XXXXXX-E).\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier that was used for the request.\"\n    },\n    \"subTopicCode\": {\n      \"type\": \"string\",\n      \"description\": \"Codes for the General, Mandatory and Additional PAI indicators\"\n    },\n    \"subTopicName\": {\n      \"type\": \"string\",\n      \"description\": \"Names for the General, Mandatory and Additional PAI indicators\"\n    },\n    \"indicatorType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of indicator - General, Additional & Mandatory\"\n    },\n    \"periodEndDate\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The Reporting period end date expressed in YYYY-MM-DD format\"\n    },\n    \"reportingPeriod\": {\n      \"type\": \"string\",\n      \"description\": \"The reporting period of the company expressed in YYYY format\"\n    },\n    \"standardizedUnit\": {\n      \"type\": \"string\",\n      \"description\": \"The units of measurements for the indicators\"\n    },\n    \"standardizedValue\": {\n      \"type\": \"string\",\n      \"description\": \"The PAI calculations based on the company-reported data, some metrics sourced from Factset Databases and Truvalue SASB Spotlights\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-esg-sfdr-pai-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: sfdrPai
---
