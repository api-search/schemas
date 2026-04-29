---
description: Action to realise on a transaction.
layout: schema
name: TransactionAction
properties_list: []
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-transaction-action-schema.json
slug: terminal-transaction-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-transaction-action-schema.json\",\n  \"title\": \"TransactionAction\",\n  \"description\": \"Action to realise on a transaction.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"AbortTransaction\",\n    \"StartTransaction\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-transaction-action-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransactionAction
---
