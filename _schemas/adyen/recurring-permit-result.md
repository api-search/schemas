---
description: PermitResult schema from Adyen API
layout: schema
name: PermitResult
properties_list:
- description: The key to link permit requests to permit results.
  name: resultKey
  type: string
- description: The permit token which is used to make payments by the partner company.
  name: token
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/recurring-permit-result-schema.json
slug: recurring-permit-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-permit-result-schema.json\",\n  \"title\": \"PermitResult\",\n  \"description\": \"PermitResult schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resultKey\": {\n      \"x-addedInVersion\": \"32\",\n      \"description\": \"The key to link permit requests to permit results.\",\n      \"type\": \"string\"\n    },\n    \"token\": {\n      \"x-addedInVersion\": \"32\",\n      \"description\": \"The permit token which is used to make payments by the partner company.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-permit-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PermitResult
---
