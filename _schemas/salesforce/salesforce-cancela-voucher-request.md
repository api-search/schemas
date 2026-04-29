---
description: ''
layout: schema
name: CancelaVoucherRequest
properties_list:
- description: ''
  name: processParameters
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-cancela-voucher-request-schema.json
slug: salesforce-cancela-voucher-request
source_filename: salesforce-cancela-voucher-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"processParameters\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"MemberId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"VoucherId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          }\n        },\n        \"required\": [\n          \"MemberId\",\n          \"VoucherId\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"processParameters\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CancelaVoucherRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-cancela-voucher-request-schema.json
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
title: CancelaVoucherRequest
---
