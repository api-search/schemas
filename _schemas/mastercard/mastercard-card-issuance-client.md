---
description: ''
layout: schema
name: Client
properties_list:
- description: Indicates whether client is VIP person. false (Default) indicates Normal client and true indicates VIP client. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* <
  name: vip
  type: boolean
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-client-schema.json
slug: mastercard-card-issuance-client
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Client\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vip\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether client is VIP person. false (Default) indicates Normal client and true indicates VIP client. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-client-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Client
---
