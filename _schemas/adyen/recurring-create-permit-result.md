---
description: CreatePermitResult schema from Adyen API
layout: schema
name: CreatePermitResult
properties_list:
- description: List of new permits.
  name: permitResultList
  type: array
- description: A unique reference associated with the request. This value is globally unique; quote it when communicating with us about this request.
  name: pspReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/recurring-create-permit-result-schema.json
slug: recurring-create-permit-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-create-permit-result-schema.json\",\n  \"title\": \"CreatePermitResult\",\n  \"description\": \"CreatePermitResult schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"permitResultList\": {\n      \"description\": \"List of new permits.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PermitResult\"\n      },\n      \"type\": \"array\"\n    },\n    \"pspReference\": {\n      \"description\": \"A unique reference associated with the request. This value is globally unique; quote it when communicating with us about this request.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-create-permit-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CreatePermitResult
---
