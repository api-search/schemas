---
description: PaginatedAccountHoldersResponse schema from Adyen API
layout: schema
name: PaginatedAccountHoldersResponse
properties_list:
- description: List of account holders.
  name: accountHolders
  type: array
- description: Indicates whether there are more items on the next page.
  name: hasNext
  type: boolean
- description: Indicates whether there are more items on the previous page.
  name: hasPrevious
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-paginated-account-holders-response-schema.json
slug: configuration-paginated-account-holders-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-paginated-account-holders-response-schema.json\",\n  \"title\": \"PaginatedAccountHoldersResponse\",\n  \"description\": \"PaginatedAccountHoldersResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolders\": {\n      \"description\": \"List of account holders.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AccountHolder\"\n      },\n      \"type\": \"array\"\n    },\n    \"hasNext\": {\n      \"description\": \"Indicates whether there are more items on the next page.\",\n      \"type\": \"boolean\"\n    },\n    \"hasPrevious\": {\n      \"description\": \"Indicates whether there are more items on the previous page.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"accountHolders\",\n    \"hasPrevious\",\n    \"hasNext\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-paginated-account-holders-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaginatedAccountHoldersResponse
---
