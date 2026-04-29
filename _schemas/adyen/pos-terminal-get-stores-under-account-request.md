---
description: GetStoresUnderAccountRequest schema from Adyen API
layout: schema
name: GetStoresUnderAccountRequest
properties_list:
- description: The company account. If you only specify this parameter, the response includes the stores of all merchant accounts that are associated with the company account.
  name: companyAccount
  type: string
- description: The merchant account. With this parameter, the response only includes the stores of the specified merchant account.
  name: merchantAccount
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/pos-terminal-get-stores-under-account-request-schema.json
slug: pos-terminal-get-stores-under-account-request
source_filename: pos-terminal-get-stores-under-account-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/pos-terminal-get-stores-under-account-request-schema.json\",\n  \"title\": \"GetStoresUnderAccountRequest\",\n  \"description\": \"GetStoresUnderAccountRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyAccount\": {\n      \"description\": \"The company account. If you only specify this parameter, the response includes the stores of all merchant accounts that are associated with the company account.\",\n      \"type\": \"string\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account. With this parameter, the response only includes the stores of the specified merchant account.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"companyAccount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/pos-terminal-get-stores-under-account-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GetStoresUnderAccountRequest
---
