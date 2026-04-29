---
description: DeletePayoutMethodRequest schema from Adyen API
layout: schema
name: DeletePayoutMethodRequest
properties_list:
- description: The code of the account holder, from which to delete the payout methods.
  name: accountHolderCode
  type: string
- description: The codes of the payout methods to be deleted.
  name: payoutMethodCodes
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-delete-payout-method-request-schema.json
slug: accounts-delete-payout-method-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-delete-payout-method-request-schema.json\",\n  \"title\": \"DeletePayoutMethodRequest\",\n  \"description\": \"DeletePayoutMethodRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"The code of the account holder, from which to delete the payout methods.\",\n      \"type\": \"string\"\n    },\n    \"payoutMethodCodes\": {\n      \"description\": \"The codes of the payout methods to be deleted.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"accountHolderCode\",\n    \"payoutMethodCodes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-delete-payout-method-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DeletePayoutMethodRequest
---
