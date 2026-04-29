---
description: RequestActivationResponse schema from Adyen API
layout: schema
name: RequestActivationResponse
properties_list:
- description: The unique identifier of the company account.
  name: companyId
  type: string
- description: The unique identifier of the merchant account you requested to activate.
  name: merchantId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-request-activation-response-schema.json
slug: management-request-activation-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-request-activation-response-schema.json\",\n  \"title\": \"RequestActivationResponse\",\n  \"description\": \"RequestActivationResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyId\": {\n      \"description\": \"The unique identifier of the company account.\",\n      \"type\": \"string\"\n    },\n    \"merchantId\": {\n      \"description\": \"The unique identifier of the merchant account you requested to activate.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-request-activation-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: RequestActivationResponse
---
