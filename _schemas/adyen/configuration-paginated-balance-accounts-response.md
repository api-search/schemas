---
description: PaginatedBalanceAccountsResponse schema from Adyen API
layout: schema
name: PaginatedBalanceAccountsResponse
properties_list:
- description: List of balance accounts.
  name: balanceAccounts
  type: array
- description: Indicates whether there are more items on the next page.
  name: hasNext
  type: boolean
- description: Indicates whether there are more items on the previous page.
  name: hasPrevious
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-paginated-balance-accounts-response-schema.json
slug: configuration-paginated-balance-accounts-response
source_filename: configuration-paginated-balance-accounts-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-paginated-balance-accounts-response-schema.json\",\n  \"title\": \"PaginatedBalanceAccountsResponse\",\n  \"description\": \"PaginatedBalanceAccountsResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"balanceAccounts\": {\n      \"description\": \"List of balance accounts.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/BalanceAccountBase\"\n      },\n      \"type\": \"array\"\n    },\n    \"hasNext\": {\n      \"description\": \"Indicates whether there are more items on the next page.\",\n      \"type\": \"boolean\"\n    },\n    \"hasPrevious\": {\n      \"description\": \"Indicates whether there are more items on the previous page.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"balanceAccounts\",\n    \"hasPrevious\",\n \
  \   \"hasNext\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-paginated-balance-accounts-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaginatedBalanceAccountsResponse
---
