---
description: Mobile number details
layout: schema
name: Mobile
properties_list:
- description: 'ISD code is defined as the country code to call a mobile subscriber directly from outside the country. For example, +91 for India and +971 for UAE. <BR/>If not provided, then the institution ISD code '
  name: isd
  type: string
- description: Mobile number excluding ISD Code. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required when SMS alert is activated or ISD value is provided.
  name: number
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-mobile-schema.json
slug: mastercard-card-issuance-mobile
source_filename: mastercard-card-issuance-mobile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Mobile\",\n  \"type\": \"object\",\n  \"description\": \"Mobile number details\",\n  \"properties\": {\n    \"isd\": {\n      \"type\": \"string\",\n      \"description\": \"ISD code is defined as the country code to call a mobile subscriber directly from outside the country. For example, +91 for India and +971 for UAE. <BR/>If not provided, then the institution ISD code is populated.\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"Mobile number excluding ISD Code. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required when SMS alert is activated or ISD value is provided.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-mobile-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Mobile
---
