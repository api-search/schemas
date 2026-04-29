---
description: ThreeDS2ResultRequest schema from Adyen API
layout: schema
name: ThreeDS2ResultRequest
properties_list:
- description: The merchant account identifier, with which you want to process the transaction.
  name: merchantAccount
  type: string
- description: The pspReference returned in the /authorise call.
  name: pspReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-three-ds2-result-request-schema.json
slug: payments-three-ds2-result-request
source_filename: payments-three-ds2-result-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-three-ds2-result-request-schema.json\",\n  \"title\": \"ThreeDS2ResultRequest\",\n  \"description\": \"ThreeDS2ResultRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier, with which you want to process the transaction.\",\n      \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"description\": \"The pspReference returned in the /authorise call.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\",\n    \"pspReference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-three-ds2-result-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ThreeDS2ResultRequest
---
