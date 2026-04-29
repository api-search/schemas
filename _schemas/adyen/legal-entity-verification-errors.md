---
description: VerificationErrors schema from Adyen API
layout: schema
name: VerificationErrors
properties_list:
- description: List of the verification errors.
  name: problems
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-verification-errors-schema.json
slug: legal-entity-verification-errors
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-verification-errors-schema.json\",\n  \"title\": \"VerificationErrors\",\n  \"description\": \"VerificationErrors schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"problems\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"List of the verification errors.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CapabilityProblem\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-verification-errors-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: VerificationErrors
---
