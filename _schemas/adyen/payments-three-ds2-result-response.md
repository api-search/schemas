---
description: ThreeDS2ResultResponse schema from Adyen API
layout: schema
name: ThreeDS2ResultResponse
properties_list:
- description: The result of the 3D Secure 2 authentication.
  name: threeDS2Result
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-three-ds2-result-response-schema.json
slug: payments-three-ds2-result-response
source_filename: payments-three-ds2-result-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-three-ds2-result-response-schema.json\",\n  \"title\": \"ThreeDS2ResultResponse\",\n  \"description\": \"ThreeDS2ResultResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"threeDS2Result\": {\n      \"description\": \"The result of the 3D Secure 2 authentication.\",\n      \"$ref\": \"#/components/schemas/ThreeDS2Result\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-three-ds2-result-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ThreeDS2ResultResponse
---
