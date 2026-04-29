---
description: Status of created Merchant
layout: schema
name: ValidationStatus
properties_list:
- description: List of validation messages for a merchant.
  name: messages
  type: array
- description: Ethoca's CX team contact
  name: contactUs
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-validation-status-schema.json
slug: mastercard-ethoca-merchant-self-services-validation-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ValidationStatus\",\n  \"type\": \"object\",\n  \"description\": \"Status of created Merchant\",\n  \"properties\": {\n    \"messages\": {\n      \"type\": \"array\",\n      \"description\": \"List of validation messages for a merchant.\"\n    },\n    \"contactUs\": {\n      \"type\": \"string\",\n      \"description\": \"Ethoca's CX team contact\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-validation-status-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: ValidationStatus
---
