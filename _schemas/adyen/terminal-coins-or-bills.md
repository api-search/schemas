---
description: Indicates the remaining number of coins or bills of a given value in a cash handling device. When the cash handling machine does not have any more coins or bills of a certain value, the number must be equal to 0. Number of coins or bills of a given value.
layout: schema
name: CoinsOrBills
properties_list:
- description: Value of a coin or bill.
  name: UnitValue
  type: number
- description: Number of elements.
  name: Number
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-coins-or-bills-schema.json
slug: terminal-coins-or-bills
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-coins-or-bills-schema.json\",\n  \"title\": \"CoinsOrBills\",\n  \"description\": \"Indicates the remaining number of coins or bills of a given value in a cash handling device. When the cash handling machine does not have any more coins or bills of a certain value, the number must be equal to 0. Number of coins or bills of a given value.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UnitValue\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0,\n      \"description\": \"Value of a coin or bill.\"\n    },\n    \"Number\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of elements.\"\n    }\n  },\n  \"required\": [\n    \"UnitValue\",\n    \"Number\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-coins-or-bills-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CoinsOrBills
---
