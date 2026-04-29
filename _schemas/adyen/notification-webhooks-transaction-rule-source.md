---
description: TransactionRuleSource schema from Adyen API
layout: schema
name: TransactionRuleSource
properties_list:
- description: ID of the resource, when applicable.
  name: id
  type: string
- description: 'Indicates the type of resource for which the transaction rule is defined. Possible values: * **PaymentInstrumentGroup** * **PaymentInstrument** * **BalancePlatform** * **EntityUsageConfiguration** * *'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-transaction-rule-source-schema.json
slug: notification-webhooks-transaction-rule-source
source_filename: notification-webhooks-transaction-rule-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-transaction-rule-source-schema.json\",\n  \"title\": \"TransactionRuleSource\",\n  \"description\": \"TransactionRuleSource schema from Adyen API\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"ID of the resource, when applicable.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"Indicates the type of resource for which the transaction rule is defined.\\n\\nPossible values:\\n\\n * **PaymentInstrumentGroup**\\n\\n* **PaymentInstrument**\\n\\n* **BalancePlatform**\\n\\n* **EntityUsageConfiguration**\\n\\n* **PlatformRule**: The transaction rule is a platform-wide rule imposed by Adyen.\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-transaction-rule-source-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransactionRuleSource
---
