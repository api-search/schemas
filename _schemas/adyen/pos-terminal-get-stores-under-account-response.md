---
description: GetStoresUnderAccountResponse schema from Adyen API
layout: schema
name: GetStoresUnderAccountResponse
properties_list:
- description: Array that returns a list of all stores for the specified merchant account, or for all merchant accounts under the company account.
  name: stores
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/pos-terminal-get-stores-under-account-response-schema.json
slug: pos-terminal-get-stores-under-account-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/pos-terminal-get-stores-under-account-response-schema.json\",\n  \"title\": \"GetStoresUnderAccountResponse\",\n  \"description\": \"GetStoresUnderAccountResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stores\": {\n      \"description\": \"Array that returns a list of all stores for the specified merchant account, or for all merchant accounts under the company account.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Store\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/pos-terminal-get-stores-under-account-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GetStoresUnderAccountResponse
---
