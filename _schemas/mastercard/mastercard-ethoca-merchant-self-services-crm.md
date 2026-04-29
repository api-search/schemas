---
description: Customer Relationship Management
layout: schema
name: Crm
properties_list:
- description: Confirmation of payment account setup
  name: paymentConfirmation
  type: boolean
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-crm-schema.json
slug: mastercard-ethoca-merchant-self-services-crm
source_filename: mastercard-ethoca-merchant-self-services-crm-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Crm\",\n  \"type\": \"object\",\n  \"description\": \"Customer Relationship Management\",\n  \"properties\": {\n    \"paymentConfirmation\": {\n      \"type\": \"boolean\",\n      \"description\": \"Confirmation of payment account setup\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-crm-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Crm
---
