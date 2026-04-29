---
description: AuthenticationResultRequest schema from Adyen API
layout: schema
name: AuthenticationResultRequest
properties_list:
- description: The merchant account identifier, with which the authentication was processed.
  name: merchantAccount
  type: string
- description: The pspReference identifier for the transaction.
  name: pspReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-authentication-result-request-schema.json
slug: payments-authentication-result-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-authentication-result-request-schema.json\",\n  \"title\": \"AuthenticationResultRequest\",\n  \"description\": \"AuthenticationResultRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier, with which the authentication was processed.\",\n      \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"description\": \"The pspReference identifier for the transaction.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\",\n    \"pspReference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-authentication-result-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AuthenticationResultRequest
---
