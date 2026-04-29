---
description: TransactionRuleEntityKey schema from Adyen API
layout: schema
name: TransactionRuleEntityKey
properties_list:
- description: The unique identifier of the resource.
  name: entityReference
  type: string
- description: 'The type of resource. Possible values: **balancePlatform**, **paymentInstrumentGroup**, **accountHolder**, **balanceAccount**, or **paymentInstrument**.'
  name: entityType
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-transaction-rule-entity-key-schema.json
slug: configuration-transaction-rule-entity-key
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-transaction-rule-entity-key-schema.json\",\n  \"title\": \"TransactionRuleEntityKey\",\n  \"description\": \"TransactionRuleEntityKey schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entityReference\": {\n      \"description\": \"The unique identifier of the resource.\",\n      \"type\": \"string\"\n    },\n    \"entityType\": {\n      \"description\": \"The type of resource.\\n\\nPossible values: **balancePlatform**, **paymentInstrumentGroup**, **accountHolder**, **balanceAccount**, or **paymentInstrument**.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-transaction-rule-entity-key-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransactionRuleEntityKey
---
