---
description: StoredValueAccountStatus schema from Adyen API
layout: schema
name: StoredValueAccountStatus
properties_list:
- description: ''
  name: StoredValueAccountID
  type: object
- description: ''
  name: CurrentBalance
  type: number
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-stored-value-account-status-schema.json
slug: terminal-stored-value-account-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-stored-value-account-status-schema.json\",\n  \"title\": \"StoredValueAccountStatus\",\n  \"description\": \"StoredValueAccountStatus schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StoredValueAccountID\": {\n      \"$ref\": \"#/components/schemas/StoredValueAccountID\"\n    },\n    \"CurrentBalance\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    }\n  },\n  \"required\": [\n    \"StoredValueAccountID\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-stored-value-account-status-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: StoredValueAccountStatus
---
