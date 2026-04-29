---
description: Paginated list of payment overdues
layout: schema
name: OverdueList
properties_list:
- description: List of payment overdue records
  name: data
  type: array
provider_name: Allianz Trade
provider_slug: allianz-trade-online
schema_file: json-schema/trade-payment-overdues-overdue_list-schema.json
slug: trade-payment-overdues-overdue_list
source_filename: trade-payment-overdues-overdue_list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.allianz-trade.com/schemas/trade-payment-overdues-overdue_list-schema.json\",\n  \"title\": \"OverdueList\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of payment overdues\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"List of payment overdue records\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Overdue\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/json-schema/trade-payment-overdues-overdue_list-schema.json
tags:
- Credit Insurance
- Insurance
- Risk Management
- Trade Credit
- E-Commerce
- Surety
title: OverdueList
---
