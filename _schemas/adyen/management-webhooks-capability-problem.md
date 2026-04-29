---
description: CapabilityProblem schema from Adyen API
layout: schema
name: CapabilityProblem
properties_list:
- description: The ID and the type of entity that has verification errors.
  name: entity
  type: object
- description: List of verification errors.
  name: verificationErrors
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-webhooks-capability-problem-schema.json
slug: management-webhooks-capability-problem
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-webhooks-capability-problem-schema.json\",\n  \"title\": \"CapabilityProblem\",\n  \"description\": \"CapabilityProblem schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entity\": {\n      \"description\": \"The ID and the type of entity that has verification errors.\",\n      \"$ref\": \"#/components/schemas/CapabilityProblemEntity\"\n    },\n    \"verificationErrors\": {\n      \"description\": \"List of verification errors.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/VerificationError\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-webhooks-capability-problem-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CapabilityProblem
---
