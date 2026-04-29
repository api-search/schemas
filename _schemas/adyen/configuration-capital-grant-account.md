---
description: CapitalGrantAccount schema from Adyen API
layout: schema
name: CapitalGrantAccount
properties_list:
- description: The balances of the grant account.
  name: balances
  type: array
- description: The unique identifier of the balance account used to fund the grant.
  name: fundingBalanceAccountId
  type: string
- description: The identifier of the grant account.
  name: id
  type: string
- description: The limits of the grant account.
  name: limits
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-capital-grant-account-schema.json
slug: configuration-capital-grant-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-capital-grant-account-schema.json\",\n  \"title\": \"CapitalGrantAccount\",\n  \"description\": \"CapitalGrantAccount schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"balances\": {\n      \"description\": \"The balances of the grant account.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CapitalBalance\"\n      },\n      \"type\": \"array\"\n    },\n    \"fundingBalanceAccountId\": {\n      \"description\": \"The unique identifier of the balance account used to fund the grant.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The identifier of the grant account.\",\n      \"type\": \"string\"\n    },\n    \"limits\": {\n      \"description\": \"The limits of the grant account.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/GrantLimit\"\
  \n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-capital-grant-account-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CapitalGrantAccount
---
