---
description: CapabilityProblem schema from Adyen API
layout: schema
name: CapabilityProblem
properties_list:
- description: ''
  name: entity
  type: object
- description: ''
  name: verificationErrors
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-capability-problem-schema.json
slug: legal-entity-capability-problem
source_filename: legal-entity-capability-problem-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-capability-problem-schema.json\",\n  \"title\": \"CapabilityProblem\",\n  \"description\": \"CapabilityProblem schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entity\": {\n      \"$ref\": \"#/components/schemas/CapabilityProblemEntity\"\n    },\n    \"verificationErrors\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/VerificationError\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-capability-problem-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CapabilityProblem
---
