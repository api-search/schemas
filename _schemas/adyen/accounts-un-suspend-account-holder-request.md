---
description: UnSuspendAccountHolderRequest schema from Adyen API
layout: schema
name: UnSuspendAccountHolderRequest
properties_list:
- description: The code of the account holder to be reinstated.
  name: accountHolderCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-un-suspend-account-holder-request-schema.json
slug: accounts-un-suspend-account-holder-request
source_filename: accounts-un-suspend-account-holder-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-un-suspend-account-holder-request-schema.json\",\n  \"title\": \"UnSuspendAccountHolderRequest\",\n  \"description\": \"UnSuspendAccountHolderRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"The code of the account holder to be reinstated.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"accountHolderCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-un-suspend-account-holder-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UnSuspendAccountHolderRequest
---
