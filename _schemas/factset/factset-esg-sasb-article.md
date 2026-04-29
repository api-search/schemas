---
description: ''
layout: schema
name: sasbArticle
properties_list:
- description: Date of article based on dateOf parameter
  name: date
  type: string
- description: FactSet Entity Identifier. Six alpha-numeric characters, excluding vowels, with a -E suffix (XXXXXX-E).
  name: fsymId
  type: string
- description: Identifier that was used for the request.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-esg-sasb-article-schema.json
slug: factset-esg-sasb-article
source_filename: factset-esg-sasb-article-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"sasbArticle\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"Date of article based on dateOf parameter\"\n    },\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Entity Identifier. Six alpha-numeric characters, excluding vowels, with a -E suffix (XXXXXX-E).\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier that was used for the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-esg-sasb-article-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: sasbArticle
---
