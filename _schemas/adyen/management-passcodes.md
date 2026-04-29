---
description: Passcodes schema from Adyen API
layout: schema
name: Passcodes
properties_list:
- description: The passcode for the Admin menu and the Settings menu.
  name: adminMenuPin
  type: string
- description: The passcode for referenced and unreferenced refunds on standalone terminals.
  name: refundPin
  type: string
- description: The passcode to unlock the terminal screen after a timeout.
  name: screenLockPin
  type: string
- description: The passcode for the Transactions menu.
  name: txMenuPin
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-passcodes-schema.json
slug: management-passcodes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-passcodes-schema.json\",\n  \"title\": \"Passcodes\",\n  \"description\": \"Passcodes schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"adminMenuPin\": {\n      \"description\": \"The passcode for the Admin menu and the Settings menu.\",\n      \"maxLength\": 6,\n      \"type\": \"string\"\n    },\n    \"refundPin\": {\n      \"description\": \"The passcode for referenced and unreferenced refunds on standalone terminals.\",\n      \"maxLength\": 6,\n      \"type\": \"string\"\n    },\n    \"screenLockPin\": {\n      \"description\": \"The passcode to unlock the terminal screen after a timeout.\",\n      \"maxLength\": 6,\n      \"minLength\": 4,\n      \"type\": \"string\"\n    },\n    \"txMenuPin\": {\n      \"description\": \"The passcode for the Transactions menu.\",\n \
  \     \"maxLength\": 6,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-passcodes-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Passcodes
---
