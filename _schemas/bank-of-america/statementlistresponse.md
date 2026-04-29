---
description: List of available statements
layout: schema
name: StatementListResponse
properties_list:
- description: ''
  name: statements
  type: array
- description: ''
  name: totalCount
  type: integer
provider_name: Bank of America
provider_slug: bank-of-america
schema_file: json-schema/statementlistresponse-schema.json
slug: statementlistresponse
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-america/json-schema/statementlistresponse-schema.json\",\n  \"title\": \"StatementListResponse\",\n  \"type\": \"object\",\n  \"description\": \"List of available statements\",\n  \"properties\": {\n    \"statements\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Statement\"\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-america/refs/heads/main/json-schema/statementlistresponse-schema.json
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
title: StatementListResponse
---
