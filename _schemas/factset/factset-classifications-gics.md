---
description: ''
layout: schema
name: gics
properties_list:
- description: FactSet Entity Identifier by default, otherwise returns FactSet Regional Identifier. This is a six alpha-numeric characters, excluding vowels, with an -E suffix (XXXXXX-E).
  name: fsymId
  type: string
- description: Date in YYYY-MM-DD for the classification record from GICS Direct
  name: date
  type: string
- description: GICS Sector Name in Proper Format.
  name: gicsSectorName
  type: string
- description: GICS Sector Number
  name: gicsSectorNumber
  type: string
- description: GICS Industry Group Name in Proper Format.
  name: gicsIndustryGroupName
  type: string
- description: GICS Industry Group Number
  name: gicsIndustryGroupNumber
  type: string
- description: GICS Industry Name in Proper Format.
  name: gicsIndustryName
  type: string
- description: GICS Industry Number
  name: gicsIndustryNumber
  type: string
- description: GICS Sub-Industry Name in Proper Format.
  name: gicsSubIndustryName
  type: string
- description: GICS Industry Number.
  name: gicsSubIndustryNumber
  type: string
- description: Identifier specified in the request
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-classifications-gics-schema.json
slug: factset-classifications-gics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"gics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Entity Identifier by default, otherwise returns FactSet Regional Identifier. This is a six alpha-numeric characters, excluding vowels, with an -E suffix (XXXXXX-E).\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"Date in YYYY-MM-DD for the classification record from GICS Direct\"\n    },\n    \"gicsSectorName\": {\n      \"type\": \"string\",\n      \"description\": \"GICS Sector Name in Proper Format.\"\n    },\n    \"gicsSectorNumber\": {\n      \"type\": \"string\",\n      \"description\": \"GICS Sector Number\"\n    },\n    \"gicsIndustryGroupName\": {\n      \"type\": \"string\",\n      \"description\": \"GICS Industry Group Name in Proper Format.\"\n    },\n    \"gicsIndustryGroupNumber\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"GICS Industry Group Number\"\n    },\n    \"gicsIndustryName\": {\n      \"type\": \"string\",\n      \"description\": \"GICS Industry Name in Proper Format.\"\n    },\n    \"gicsIndustryNumber\": {\n      \"type\": \"string\",\n      \"description\": \"GICS Industry Number\"\n    },\n    \"gicsSubIndustryName\": {\n      \"type\": \"string\",\n      \"description\": \"GICS Sub-Industry Name in Proper Format.\"\n    },\n    \"gicsSubIndustryNumber\": {\n      \"type\": \"string\",\n      \"description\": \"GICS Industry Number.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier specified in the request\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-classifications-gics-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: gics
---
