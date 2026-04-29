---
description: GetAccountHolderRequest schema from Adyen API
layout: schema
name: GetAccountHolderRequest
properties_list:
- description: The code of the account of which to retrieve the details. > Required if no `accountHolderCode` is provided.
  name: accountCode
  type: string
- description: The code of the account holder of which to retrieve the details. > Required if no `accountCode` is provided.
  name: accountHolderCode
  type: string
- description: True if the request should return the account holder details
  name: showDetails
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-get-account-holder-request-schema.json
slug: accounts-get-account-holder-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-get-account-holder-request-schema.json\",\n  \"title\": \"GetAccountHolderRequest\",\n  \"description\": \"GetAccountHolderRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountCode\": {\n      \"description\": \"The code of the account of which to retrieve the details.\\n> Required if no `accountHolderCode` is provided.\",\n      \"type\": \"string\"\n    },\n    \"accountHolderCode\": {\n      \"description\": \"The code of the account holder of which to retrieve the details.\\n> Required if no `accountCode` is provided.\",\n      \"type\": \"string\"\n    },\n    \"showDetails\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"True if the request should return the account holder details\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-get-account-holder-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GetAccountHolderRequest
---
