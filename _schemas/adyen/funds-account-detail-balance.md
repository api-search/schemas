---
description: AccountDetailBalance schema from Adyen API
layout: schema
name: AccountDetailBalance
properties_list:
- description: The code of the account that holds the balance.
  name: accountCode
  type: string
- description: Details of the balance held by the account.
  name: detailBalance
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/funds-account-detail-balance-schema.json
slug: funds-account-detail-balance
source_filename: funds-account-detail-balance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-account-detail-balance-schema.json\",\n  \"title\": \"AccountDetailBalance\",\n  \"description\": \"AccountDetailBalance schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountCode\": {\n      \"description\": \"The code of the account that holds the balance.\",\n      \"type\": \"string\"\n    },\n    \"detailBalance\": {\n      \"description\": \"Details of the balance held by the account.\",\n      \"$ref\": \"#/components/schemas/DetailBalance\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-account-detail-balance-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountDetailBalance
---
