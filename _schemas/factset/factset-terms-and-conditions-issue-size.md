---
description: Issue Size Data Items for a Fixed Income security.
layout: schema
name: issueSize
properties_list:
- description: Security identifier used in the request.
  name: requestId
  type: string
- description: FactSet Permanent Security Identifier.
  name: fsymId
  type: string
- description: Amount Outstanding Effective Date (out_amt_eff_date)
  name: outAmtEffDate
  type: string
- description: Amount Outstanding Currency
  name: outAmtCurrency
  type: string
- description: Amount Outstanding
  name: outAmt
  type: number
- description: Amount Outstanding Action Amount
  name: outAmtChange
  type: number
- description: Price - Amount Outstanding Action
  name: outAmtChangePrice
  type: number
- description: Amount Outstanding Action Type
  name: outAmtChangeType
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-terms-and-conditions-issue-size-schema.json
slug: factset-terms-and-conditions-issue-size
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"issueSize\",\n  \"type\": \"object\",\n  \"description\": \"Issue Size Data Items for a Fixed Income security.\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Security identifier used in the request.\"\n    },\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Permanent Security Identifier.\"\n    },\n    \"outAmtEffDate\": {\n      \"type\": \"string\",\n      \"description\": \"Amount Outstanding Effective Date (out_amt_eff_date)\"\n    },\n    \"outAmtCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"Amount Outstanding Currency\"\n    },\n    \"outAmt\": {\n      \"type\": \"number\",\n      \"description\": \"Amount Outstanding\"\n    },\n    \"outAmtChange\": {\n      \"type\": \"number\",\n      \"description\": \"Amount Outstanding Action Amount\"\n    },\n    \"outAmtChangePrice\":\
  \ {\n      \"type\": \"number\",\n      \"description\": \"Price - Amount Outstanding Action\"\n    },\n    \"outAmtChangeType\": {\n      \"type\": \"string\",\n      \"description\": \"Amount Outstanding Action Type\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-terms-and-conditions-issue-size-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: issueSize
---
