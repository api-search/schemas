---
description: SubjectErasureResponse schema from Adyen API
layout: schema
name: SubjectErasureResponse
properties_list:
- description: The result of this operation.
  name: result
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/data-protection-subject-erasure-response-schema.json
slug: data-protection-subject-erasure-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/data-protection-subject-erasure-response-schema.json\",\n  \"title\": \"SubjectErasureResponse\",\n  \"description\": \"SubjectErasureResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"result\": {\n      \"description\": \"The result of this operation.\",\n      \"enum\": [\n        \"ACTIVE_RECURRING_TOKEN_EXISTS\",\n        \"ALREADY_PROCESSED\",\n        \"PAYMENT_NOT_FOUND\",\n        \"SUCCESS\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/data-protection-subject-erasure-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SubjectErasureResponse
---
