---
description: ''
layout: schema
name: IssueaVoucherRequest
properties_list:
- description: ''
  name: processParameters
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-issuea-voucher-request-schema.json
slug: salesforce-issuea-voucher-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"processParameters\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"MemberId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"VoucherCode\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"VoucherFaceValue\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"VoucherExpirationDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"MemberId\",\n          \"VoucherCode\",\n          \"VoucherFaceValue\",\n          \"VoucherExpirationDate\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"processParameters\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"IssueaVoucherRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-issuea-voucher-request-schema.json
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
title: IssueaVoucherRequest
---
