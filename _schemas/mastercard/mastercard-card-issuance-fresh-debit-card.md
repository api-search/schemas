---
description: Debit Card Details. <BR/>card number or card id or card packId must exist while issuing existing non personalized card.
layout: schema
name: FreshDebitCard
properties_list:
- description: Indicates whether existing non-personalized card is being issued.
  name: nonPersonalized
  type: boolean
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-fresh-debit-card-schema.json
slug: mastercard-card-issuance-fresh-debit-card
source_filename: mastercard-card-issuance-fresh-debit-card-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FreshDebitCard\",\n  \"type\": \"object\",\n  \"description\": \"Debit Card Details. <BR/>card number or card id or card packId must exist while issuing existing non personalized card.\",\n  \"properties\": {\n    \"nonPersonalized\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether existing non-personalized card is being issued.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-fresh-debit-card-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: FreshDebitCard
---
