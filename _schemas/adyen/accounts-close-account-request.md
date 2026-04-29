---
description: CloseAccountRequest schema from Adyen API
layout: schema
name: CloseAccountRequest
properties_list:
- description: The code of account to be closed.
  name: accountCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-close-account-request-schema.json
slug: accounts-close-account-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-close-account-request-schema.json\",\n  \"title\": \"CloseAccountRequest\",\n  \"description\": \"CloseAccountRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountCode\": {\n      \"description\": \"The code of account to be closed.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"accountCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-close-account-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CloseAccountRequest
---
