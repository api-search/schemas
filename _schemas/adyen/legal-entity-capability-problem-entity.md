---
description: CapabilityProblemEntity schema from Adyen API
layout: schema
name: CapabilityProblemEntity
properties_list:
- description: List of document IDs corresponding to the verification errors from capabilities.
  name: documents
  type: array
- description: ''
  name: id
  type: string
- description: ''
  name: owner
  type: object
- description: ''
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-capability-problem-entity-schema.json
slug: legal-entity-capability-problem-entity
source_filename: legal-entity-capability-problem-entity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-capability-problem-entity-schema.json\",\n  \"title\": \"CapabilityProblemEntity\",\n  \"description\": \"CapabilityProblemEntity schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"documents\": {\n      \"description\": \"List of document IDs corresponding to the verification errors from capabilities.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"owner\": {\n      \"$ref\": \"#/components/schemas/CapabilityProblemEntity-recursive\"\n    },\n    \"type\": {\n      \"enum\": [\n        \"BankAccount\",\n        \"Document\",\n        \"LegalEntity\",\n        \"product\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-capability-problem-entity-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CapabilityProblemEntity
---
