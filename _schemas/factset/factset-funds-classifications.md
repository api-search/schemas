---
description: ''
layout: schema
name: classifications
properties_list:
- description: FactSet Security Identifier. Six alpha-numeric characters, excluding vowels, with a -S suffix (XXXXXX-S), resolved from the requestId of the Fund requested.
  name: fsymId
  type: string
- description: The requested Id sent as input.
  name: requestId
  type: string
- description: Returns the asset class description from FactSet's fund classification system. Asset class designates the fund's underlying holding type, e.g. equity, fixed-income, etc.
  name: assetClass
  type: string
- description: Returns the asset class category description from FactSet's fund classification system. The asset class category is the first-tier subcategory within the fund's asset class, e.g. size & style, sector,
  name: categoryClass
  type: string
- description: Returns the fund's economic development description from FactSet's fund classification system. This description refers to the development level for the fund's geographic region of focus, e.g. develope
  name: economicDevelopmentClass
  type: string
- description: Returns the fund's focus description from FactSet's fund classification system. The fund's focus is the second-tier subcategory within the fund's asset class, e.g. small cap, energy, etc.
  name: focusClass
  type: string
- description: Returns the fund's specific geography description from FactSet's fund classification system. Specific geography refers to the fund's particular geographic focus within the region, e.g. Chile, BRICs, e
  name: geographicClass
  type: string
- description: Returns the fund's niche description from FactSet's fund classification system. The fund's niche is the third-tier subcategory with the fund's asset class, e.g. growth, coal, etc.
  name: nicheClass
  type: string
- description: Returns the fund's region description from FactSet's fund classification system. Refers to the broad regional exposure of the fund's holdings, e.g. Latin America, Asia-Pacific, etc.
  name: regionClass
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-funds-classifications-schema.json
slug: factset-funds-classifications
source_filename: factset-funds-classifications-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"classifications\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Security Identifier. Six alpha-numeric characters, excluding vowels, with a -S suffix (XXXXXX-S), resolved from the requestId of the Fund requested.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"The requested Id sent as input.\"\n    },\n    \"assetClass\": {\n      \"type\": \"string\",\n      \"description\": \"Returns the asset class description from FactSet's fund classification system. Asset class designates the fund's underlying holding type, e.g. equity, fixed-income, etc.\"\n    },\n    \"categoryClass\": {\n      \"type\": \"string\",\n      \"description\": \"Returns the asset class category description from FactSet's fund classification system. The asset class category is the first-tier subcategory\
  \ within the fund's asset class, e.g. size & style, sector, precious metals, etc.\"\n    },\n    \"economicDevelopmentClass\": {\n      \"type\": \"string\",\n      \"description\": \"Returns the fund's economic development description from FactSet's fund classification system. This description refers to the development level for the fund's geographic region of focus, e.g. developed, emerging, etc.\"\n    },\n    \"focusClass\": {\n      \"type\": \"string\",\n      \"description\": \"Returns the fund's focus description from FactSet's fund classification system. The fund's focus is the second-tier subcategory within the fund's asset class, e.g. small cap, energy, etc.\"\n    },\n    \"geographicClass\": {\n      \"type\": \"string\",\n      \"description\": \"Returns the fund's specific geography description from FactSet's fund classification system. Specific geography refers to the fund's particular geographic focus within the region, e.g. Chile, BRICs, etc.\"\n    },\n    \"nicheClass\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Returns the fund's niche description from FactSet's fund classification system. The fund's niche is the third-tier subcategory with the fund's asset class, e.g. growth, coal, etc.\"\n    },\n    \"regionClass\": {\n      \"type\": \"string\",\n      \"description\": \"Returns the fund's region description from FactSet's fund classification system. Refers to the broad regional exposure of the fund's holdings, e.g. Latin America, Asia-Pacific, etc.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-funds-classifications-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: classifications
---
