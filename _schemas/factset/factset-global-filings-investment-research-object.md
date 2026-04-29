---
description: ''
layout: schema
name: InvestmentResearchObject
properties_list:
- description: Headline of the story, actual time and date of the event.
  name: headline
  type: string
- description: Provides source of the document.
  name: source
  type: string
- description: Refers to the main company a particular document refers to.
  name: primaryIds
  type: array
- description: Refers to all companies mentioned in the document. This could also include the primary company id as well.
  name: allIds
  type: array
- description: Publish date of the latest version (in ET).
  name: filingsDate
  type: string
- description: Publish time of the latest version (in ET).
  name: filingsTime
  type: string
- description: Categories are country, industry, and subject codes. This is a comma-separated list.
  name: categories
  type: array
- description: The link to download the document.
  name: filingsLink
  type: string
- description: Unique identifier for a document.
  name: documentId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-global-filings-investment-research-object-schema.json
slug: factset-global-filings-investment-research-object
source_filename: factset-global-filings-investment-research-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InvestmentResearchObject\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"headline\": {\n      \"type\": \"string\",\n      \"description\": \"Headline of the story, actual time and date of the event.\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Provides source of the document.\"\n    },\n    \"primaryIds\": {\n      \"type\": \"array\",\n      \"description\": \"Refers to the main company a particular document refers to.\"\n    },\n    \"allIds\": {\n      \"type\": \"array\",\n      \"description\": \"Refers to all companies mentioned in the document. This could also include the primary company id as well.\"\n    },\n    \"filingsDate\": {\n      \"type\": \"string\",\n      \"description\": \"Publish date of the latest version (in ET).\"\n    },\n    \"filingsTime\": {\n      \"type\": \"string\",\n      \"description\": \"Publish time of the\
  \ latest version (in ET).\"\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"description\": \"Categories are country, industry, and subject codes. This is a comma-separated list.\"\n    },\n    \"filingsLink\": {\n      \"type\": \"string\",\n      \"description\": \"The link to download the document.\"\n    },\n    \"documentId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for a document.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-global-filings-investment-research-object-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: InvestmentResearchObject
---
