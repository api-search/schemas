---
description: CapabilityProblemEntity schema from Adyen API
layout: schema
name: CapabilityProblemEntity
properties_list:
- description: The ID of the entity.
  name: id
  type: string
- description: Contains details about the owner of the entity that has an error.
  name: owner
  type: object
- description: 'Type of entity. Possible values: **LegalEntity**, **BankAccount**, **Document**.'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-capability-problem-entity-schema.json
slug: notification-webhooks-capability-problem-entity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-capability-problem-entity-schema.json\",\n  \"title\": \"CapabilityProblemEntity\",\n  \"description\": \"CapabilityProblemEntity schema from Adyen API\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"The ID of the entity.\",\n      \"type\": \"string\"\n    },\n    \"owner\": {\n      \"description\": \"Contains details about the owner of the entity that has an error.\",\n      \"$ref\": \"#/components/schemas/CapabilityProblemEntity-recursive\"\n    },\n    \"type\": {\n      \"description\": \"Type of entity. \\n\\nPossible values: **LegalEntity**, **BankAccount**, **Document**.\",\n      \"enum\": [\n        \"BankAccount\",\n        \"Document\",\n        \"LegalEntity\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-capability-problem-entity-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CapabilityProblemEntity
---
