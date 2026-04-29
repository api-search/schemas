---
description: SuspendAccountHolderRequest schema from Adyen API
layout: schema
name: SuspendAccountHolderRequest
properties_list:
- description: The code of the account holder to be suspended.
  name: accountHolderCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-suspend-account-holder-request-schema.json
slug: accounts-suspend-account-holder-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-suspend-account-holder-request-schema.json\",\n  \"title\": \"SuspendAccountHolderRequest\",\n  \"description\": \"SuspendAccountHolderRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"The code of the account holder to be suspended.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"accountHolderCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-suspend-account-holder-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SuspendAccountHolderRequest
---
