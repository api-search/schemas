---
description: Identification of a transaction for the Sale System or the POI System.
layout: schema
name: TransactionIDType
properties_list:
- description: ''
  name: TransactionID
  type: string
- description: ''
  name: TimeStamp
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-transaction-id-type-schema.json
slug: terminal-transaction-id-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-transaction-id-type-schema.json\",\n  \"title\": \"TransactionIDType\",\n  \"description\": \"Identification of a transaction for the Sale System or the POI System.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransactionID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"TimeStamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\n    \"TransactionID\",\n    \"TimeStamp\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-transaction-id-type-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransactionIDType
---
