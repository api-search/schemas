---
description: ''
layout: schema
name: MemberVouchers
properties_list:
- description: ''
  name: voucherCount
  type: integer
- description: ''
  name: vouchers
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-member-vouchers-schema.json
slug: salesforce-member-vouchers
source_filename: salesforce-member-vouchers-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"voucherCount\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"vouchers\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"voucherCount\",\n    \"vouchers\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MemberVouchers\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-member-vouchers-schema.json
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
title: MemberVouchers
---
