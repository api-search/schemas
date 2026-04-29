---
description: ''
layout: schema
name: RedeemVoucher
properties_list:
- description: ''
  name: currencyIsoCode
  type: string
- description: ''
  name: remainingAmount
  type: number
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-redeem-voucher-schema.json
slug: salesforce-redeem-voucher
source_filename: salesforce-redeem-voucher-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"currencyIsoCode\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"remainingAmount\": {\n      \"type\": \"number\",\n      \"example\": 42.5\n    }\n  },\n  \"required\": [\n    \"currencyIsoCode\",\n    \"remainingAmount\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RedeemVoucher\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-redeem-voucher-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: RedeemVoucher
---
