---
description: AccountHolderBalanceRequest schema from Adyen API
layout: schema
name: AccountHolderBalanceRequest
properties_list:
- description: The code of the Account Holder of which to retrieve the balance.
  name: accountHolderCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/funds-account-holder-balance-request-schema.json
slug: funds-account-holder-balance-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-account-holder-balance-request-schema.json\",\n  \"title\": \"AccountHolderBalanceRequest\",\n  \"description\": \"AccountHolderBalanceRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"The code of the Account Holder of which to retrieve the balance.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"accountHolderCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-account-holder-balance-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountHolderBalanceRequest
---
