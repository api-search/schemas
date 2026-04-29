---
description: ''
layout: schema
name: OptimalPortfolio
properties_list:
- description: Account path
  name: acctName
  type: string
- description: Exclude zero
  name: excludeZero
  type: boolean
- description: Archive date
  name: archiveDate
  type: string
- description: Archive action if account exists
  name: ifAcctExists
  type: string
- description: Action if ofdb date exists
  name: ifOfdbDateExists
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-northfield-portfolio-optimizer-optimal-portfolio-schema.json
slug: factset-northfield-portfolio-optimizer-optimal-portfolio
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OptimalPortfolio\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"acctName\": {\n      \"type\": \"string\",\n      \"description\": \"Account path\"\n    },\n    \"excludeZero\": {\n      \"type\": \"boolean\",\n      \"description\": \"Exclude zero\"\n    },\n    \"archiveDate\": {\n      \"type\": \"string\",\n      \"description\": \"Archive date\"\n    },\n    \"ifAcctExists\": {\n      \"type\": \"string\",\n      \"description\": \"Archive action if account exists\"\n    },\n    \"ifOfdbDateExists\": {\n      \"type\": \"string\",\n      \"description\": \"Action if ofdb date exists\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-northfield-portfolio-optimizer-optimal-portfolio-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: OptimalPortfolio
---
