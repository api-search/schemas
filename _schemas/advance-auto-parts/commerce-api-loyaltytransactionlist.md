---
description: List of loyalty transactions.
layout: schema
name: LoyaltyTransactionList
properties_list:
- description: Array of transactions.
  name: transactions
  type: array
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
schema_file: json-schema/commerce-api-loyaltytransactionlist-schema.json
slug: commerce-api-loyaltytransactionlist
source_filename: commerce-api-loyaltytransactionlist-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LoyaltyTransactionList\",\n  \"description\": \"List of loyalty transactions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactions\": {\n      \"type\": \"array\",\n      \"description\": \"Array of transactions.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/LoyaltyTransaction\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/json-schema/commerce-api-loyaltytransactionlist-schema.json
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
title: LoyaltyTransactionList
---
