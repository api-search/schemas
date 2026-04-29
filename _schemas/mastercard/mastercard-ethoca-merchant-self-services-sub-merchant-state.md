---
description: ''
layout: schema
name: SubMerchantState
properties_list:
- description: State of the Sub-Merchant
  name: state
  type: string
- description: Reason for Inactivation. Required when state is INACTIVE.
  name: inactivationReason
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-sub-merchant-state-schema.json
slug: mastercard-ethoca-merchant-self-services-sub-merchant-state
source_filename: mastercard-ethoca-merchant-self-services-sub-merchant-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubMerchantState\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State of the Sub-Merchant\"\n    },\n    \"inactivationReason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for Inactivation. Required when state is INACTIVE.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-sub-merchant-state-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: SubMerchantState
---
