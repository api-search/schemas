---
description: CloseStoresRequest schema from Adyen API
layout: schema
name: CloseStoresRequest
properties_list:
- description: The code of the account holder.
  name: accountHolderCode
  type: string
- description: List of stores to be closed.
  name: stores
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-close-stores-request-schema.json
slug: accounts-close-stores-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-close-stores-request-schema.json\",\n  \"title\": \"CloseStoresRequest\",\n  \"description\": \"CloseStoresRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"The code of the account holder.\",\n      \"type\": \"string\"\n    },\n    \"stores\": {\n      \"description\": \"List of stores to be closed.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"accountHolderCode\",\n    \"stores\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-close-stores-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CloseStoresRequest
---
