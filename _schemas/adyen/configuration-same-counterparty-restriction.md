---
description: SameCounterpartyRestriction schema from Adyen API
layout: schema
name: SameCounterpartyRestriction
properties_list:
- description: Defines how the condition must be evaluated.
  name: operation
  type: string
- description: ''
  name: value
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-same-counterparty-restriction-schema.json
slug: configuration-same-counterparty-restriction
source_filename: configuration-same-counterparty-restriction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-same-counterparty-restriction-schema.json\",\n  \"title\": \"SameCounterpartyRestriction\",\n  \"description\": \"SameCounterpartyRestriction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operation\": {\n      \"description\": \"Defines how the condition must be evaluated.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"operation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-same-counterparty-restriction-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SameCounterpartyRestriction
---
