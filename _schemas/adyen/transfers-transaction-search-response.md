---
description: TransactionSearchResponse schema from Adyen API
layout: schema
name: TransactionSearchResponse
properties_list:
- description: Contains links to the next and previous page whenever applicable.
  name: _links
  type: object
- description: Contains the transactions that match the query parameters.
  name: data
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-transaction-search-response-schema.json
slug: transfers-transaction-search-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-transaction-search-response-schema.json\",\n  \"title\": \"TransactionSearchResponse\",\n  \"description\": \"TransactionSearchResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_links\": {\n      \"description\": \"Contains links to the next and previous page whenever applicable.\",\n      \"$ref\": \"#/components/schemas/Links\"\n    },\n    \"data\": {\n      \"description\": \"Contains the transactions that match the query parameters.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Transaction\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-transaction-search-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransactionSearchResponse
---
