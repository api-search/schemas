---
description: ''
layout: schema
name: FreshCard
properties_list:
- description: Unique code of a corporate. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required if client type is `CORPORATE`.
  name: corporateCode
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-fresh-card-schema.json
slug: mastercard-card-issuance-fresh-card
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FreshCard\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"corporateCode\": {\n      \"type\": \"string\",\n      \"description\": \"Unique code of a corporate. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required if client type is `CORPORATE`.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-fresh-card-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: FreshCard
---
