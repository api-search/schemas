---
description: Indicate the status and the remaining coins and bill in a cash handling device. Status of cash handling device.
layout: schema
name: CashHandlingDevice
properties_list:
- description: Indicates if the cash handling device is working and usable.
  name: CashHandlingOKFlag
  type: boolean
- description: Currency of a monetary amount.
  name: Currency
  type: string
- description: ''
  name: CoinsOrBills
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-cash-handling-device-schema.json
slug: terminal-cash-handling-device
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-cash-handling-device-schema.json\",\n  \"title\": \"CashHandlingDevice\",\n  \"description\": \"Indicate the status and the remaining coins and bill in a cash handling device. Status of cash handling device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CashHandlingOKFlag\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if the cash handling device is working and usable.\"\n    },\n    \"Currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3,3}$\",\n      \"description\": \"Currency of a monetary amount.\"\n    },\n    \"CoinsOrBills\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CoinsOrBills\"\n      }\n    }\n  },\n  \"required\": [\n    \"CashHandlingOKFlag\",\n    \"Currency\",\n    \"CoinsOrBills\"\n \
  \ ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-cash-handling-device-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CashHandlingDevice
---
