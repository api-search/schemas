---
description: CreatePermitRequest schema from Adyen API
layout: schema
name: CreatePermitRequest
properties_list:
- description: The merchant account identifier, with which you want to process the transaction.
  name: merchantAccount
  type: string
- description: The permits to create for this recurring contract.
  name: permits
  type: array
- description: The recurring contract the new permits will use.
  name: recurringDetailReference
  type: string
- description: The shopper's reference to uniquely identify this shopper (e.g. user ID or account ID).
  name: shopperReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/recurring-create-permit-request-schema.json
slug: recurring-create-permit-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-create-permit-request-schema.json\",\n  \"title\": \"CreatePermitRequest\",\n  \"description\": \"CreatePermitRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier, with which you want to process the transaction.\",\n      \"type\": \"string\"\n    },\n    \"permits\": {\n      \"description\": \"The permits to create for this recurring contract.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Permit\"\n      },\n      \"type\": \"array\"\n    },\n    \"recurringDetailReference\": {\n      \"description\": \"The recurring contract the new permits will use.\",\n      \"type\": \"string\"\n    },\n    \"shopperReference\": {\n      \"description\": \"The shopper's reference to uniquely\
  \ identify this shopper (e.g. user ID or account ID).\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\",\n    \"shopperReference\",\n    \"recurringDetailReference\",\n    \"permits\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-create-permit-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CreatePermitRequest
---
