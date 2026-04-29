---
description: Available financing offer details for the requested purchase amount.
layout: schema
name: OfferContent
properties_list:
- description: Minimum purchase amount eligible for Affirm financing.
  name: minimum_loan_amount
  type: number
- description: Maximum purchase amount eligible for Affirm financing.
  name: maximum_loan_amount
  type: number
- description: Array of available financing term options for this amount.
  name: terms
  type: array
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/promos-offer-content-schema.json
slug: promos-offer-content
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/promos-offer-content-schema.json\",\n  \"title\": \"OfferContent\",\n  \"description\": \"Available financing offer details for the requested purchase amount.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"minimum_loan_amount\": {\n      \"type\": \"number\",\n      \"description\": \"Minimum purchase amount eligible for Affirm financing.\",\n      \"example\": 1\n    },\n    \"maximum_loan_amount\": {\n      \"type\": \"number\",\n      \"description\": \"Maximum purchase amount eligible for Affirm financing.\",\n      \"example\": 1\n    },\n    \"terms\": {\n      \"type\": \"array\",\n      \"description\": \"Array of available financing term options for this amount.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FinancingTerm\"\n      },\n      \"example\": [\n        \"example_value\"\
  \n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/promos-offer-content-schema.json
tags: []
title: OfferContent
---
