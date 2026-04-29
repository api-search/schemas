---
description: Unique value to identify a card. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Primary clientCode or cardNumber or cardId must be present in the request while requesting card for existing primary client or new add-on client. Primary cardNumber or cardId must be present in the request while requesting 'ADD_ON' or 'SUPPLEMENTARY' card.
layout: schema
name: ConditionalCardId
properties_list: []
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-conditional-card-id-schema.json
slug: mastercard-card-issuance-conditional-card-id
source_filename: mastercard-card-issuance-conditional-card-id-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConditionalCardId\",\n  \"type\": \"string\",\n  \"description\": \"Unique value to identify a card. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Primary clientCode or cardNumber or cardId must be present in the request while requesting card for existing primary client or new add-on client. Primary cardNumber or cardId must be present in the request while requesting 'ADD_ON' or 'SUPPLEMENTARY' card.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-conditional-card-id-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: ConditionalCardId
---
