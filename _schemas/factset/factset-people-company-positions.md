---
description: List of executives for the specified company identifier.
layout: schema
name: companyPositions
properties_list:
- description: FactSet Identifier for the company.
  name: fsymId
  type: string
- description: Factset Entity Identifier for the Person
  name: personId
  type: string
- description: FactSet Name of the person
  name: name
  type: string
- description: The requested Position Title
  name: title
  type: string
- description: The number of years individual is at firm. For founders, this is since inception.
  name: yearsAtFirm
  type: number
- description: The age of the person requested.
  name: age
  type: number
- description: The Gender of the person requested.
  name: gender
  type: string
- description: The requested position code.
  name: requestPosition
  type: string
- description: Original identifier used for the request.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-people-company-positions-schema.json
slug: factset-people-company-positions
source_filename: factset-people-company-positions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"companyPositions\",\n  \"type\": \"object\",\n  \"description\": \"List of executives for the specified company identifier.\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Identifier for the company.\"\n    },\n    \"personId\": {\n      \"type\": \"string\",\n      \"description\": \"Factset Entity Identifier for the Person\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Name of the person\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The requested Position Title\"\n    },\n    \"yearsAtFirm\": {\n      \"type\": \"number\",\n      \"description\": \"The number of years individual is at firm. For founders, this is since inception.\"\n    },\n    \"age\": {\n      \"type\": \"number\",\n      \"description\": \"The age of the person requested.\"\n    },\n \
  \   \"gender\": {\n      \"type\": \"string\",\n      \"description\": \"The Gender of the person requested.\"\n    },\n    \"requestPosition\": {\n      \"type\": \"string\",\n      \"description\": \"The requested position code.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Original identifier used for the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-people-company-positions-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: companyPositions
---
