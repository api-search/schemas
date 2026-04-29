---
description: LoyaltyAcquirerData schema from Adyen API
layout: schema
name: LoyaltyAcquirerData
properties_list:
- description: ''
  name: LoyaltyAcquirerID
  type: string
- description: ''
  name: ApprovalCode
  type: string
- description: ''
  name: LoyaltyTransactionID
  type: object
- description: ''
  name: HostReconciliationID
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-loyalty-acquirer-data-schema.json
slug: terminal-loyalty-acquirer-data
source_filename: terminal-loyalty-acquirer-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-loyalty-acquirer-data-schema.json\",\n  \"title\": \"LoyaltyAcquirerData\",\n  \"description\": \"LoyaltyAcquirerData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LoyaltyAcquirerID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"ApprovalCode\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"LoyaltyTransactionID\": {\n      \"$ref\": \"#/components/schemas/TransactionIDType\"\n    },\n    \"HostReconciliationID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-loyalty-acquirer-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LoyaltyAcquirerData
---
