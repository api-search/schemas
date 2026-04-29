---
description: Paginated list of insurance claims
layout: schema
name: ClaimList
properties_list:
- description: List of insurance claim records
  name: data
  type: array
provider_name: Allianz Trade
provider_slug: allianz-trade-online
schema_file: json-schema/trade-claims-claim_list-schema.json
slug: trade-claims-claim_list
source_filename: trade-claims-claim_list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.allianz-trade.com/schemas/trade-claims-claim_list-schema.json\",\n  \"title\": \"ClaimList\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of insurance claims\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"List of insurance claim records\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Claim\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/json-schema/trade-claims-claim_list-schema.json
tags:
- Credit Insurance
- Insurance
- Risk Management
- Trade Credit
- E-Commerce
- Surety
title: ClaimList
---
