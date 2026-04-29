---
description: Allows the check information to be provided by the Sale System before requesting the payment, or stored by the Sale System after processing of the payment. Information related to the paper check used for the transaction.
layout: schema
name: CheckData
properties_list:
- description: Mandatory if TrackData absent.
  name: BankID
  type: string
- description: Mandatory if TrackData absent.
  name: AccountNumber
  type: string
- description: Mandatory if TrackData absent.
  name: CheckNumber
  type: string
- description: ''
  name: TrackData
  type: object
- description: If provided by the customer.
  name: CheckCardNumber
  type: string
- description: ''
  name: TypeCode
  type: object
- description: Absent if country of the Sale system.
  name: Country
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-check-data-schema.json
slug: terminal-check-data
source_filename: terminal-check-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-check-data-schema.json\",\n  \"title\": \"CheckData\",\n  \"description\": \"Allows the check information to be provided by the Sale System before requesting the payment, or stored by the Sale System after processing of the payment. Information related to the paper check used for the transaction.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BankID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Mandatory if TrackData absent.\"\n    },\n    \"AccountNumber\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Mandatory if TrackData absent.\"\n    },\n    \"CheckNumber\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Mandatory if TrackData absent.\"\n    },\n    \"TrackData\":\
  \ {\n      \"$ref\": \"#/components/schemas/TrackData\"\n    },\n    \"CheckCardNumber\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"If provided by the customer.\"\n    },\n    \"TypeCode\": {\n      \"$ref\": \"#/components/schemas/TypeCode\"\n    },\n    \"Country\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3,3}$\",\n      \"description\": \"Absent if country of the Sale system.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-check-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CheckData
---
