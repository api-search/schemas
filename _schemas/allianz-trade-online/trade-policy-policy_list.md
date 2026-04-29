---
description: Paginated list of trade credit insurance policies
layout: schema
name: PolicyList
properties_list:
- description: List of policy records
  name: data
  type: array
provider_name: Allianz Trade
provider_slug: allianz-trade-online
schema_file: json-schema/trade-policy-policy_list-schema.json
slug: trade-policy-policy_list
source_filename: trade-policy-policy_list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.allianz-trade.com/schemas/trade-policy-policy_list-schema.json\",\n  \"title\": \"PolicyList\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of trade credit insurance policies\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"List of policy records\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Policy\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/json-schema/trade-policy-policy_list-schema.json
tags:
- Credit Insurance
- Insurance
- Risk Management
- Trade Credit
- E-Commerce
- Surety
title: PolicyList
---
