---
description: A single available financing term option including APR and payment details.
layout: schema
name: FinancingTerm
properties_list:
- description: Purchase amount this term applies to, in cents.
  name: amount
  type: integer
- description: Type of financing loan (e.g., split_pay, installment).
  name: loan_type
  type: string
- description: Annual percentage rate for this financing term.
  name: apr
  type: number
- description: Monthly installment payment amount in cents.
  name: installment_amount
  type: integer
- description: Total number of installment payments.
  name: installment_count
  type: integer
- description: Total interest charged over the life of the loan in cents.
  name: interest_amount
  type: integer
- description: Total amount paid including principal and interest, in cents.
  name: total_amount
  type: integer
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/promos-financing-term-schema.json
slug: promos-financing-term
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/promos-financing-term-schema.json\",\n  \"title\": \"FinancingTerm\",\n  \"description\": \"A single available financing term option including APR and payment details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"integer\",\n      \"description\": \"Purchase amount this term applies to, in cents.\",\n      \"example\": 1\n    },\n    \"loan_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of financing loan (e.g., split_pay, installment).\",\n      \"example\": \"standard\"\n    },\n    \"apr\": {\n      \"type\": \"number\",\n      \"description\": \"Annual percentage rate for this financing term.\",\n      \"minimum\": 0,\n      \"example\": 1\n    },\n    \"installment_amount\": {\n      \"type\": \"integer\",\n      \"description\": \"Monthly installment\
  \ payment amount in cents.\",\n      \"example\": 1\n    },\n    \"installment_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of installment payments.\",\n      \"example\": 1\n    },\n    \"interest_amount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total interest charged over the life of the loan in cents.\",\n      \"example\": 1\n    },\n    \"total_amount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total amount paid including principal and interest, in cents.\",\n      \"example\": 1\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/promos-financing-term-schema.json
tags: []
title: FinancingTerm
---
