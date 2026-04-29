---
description: ''
layout: schema
name: refundPayment
properties_list:
- description: Unique refund payment Reference of the real time settlement method provided by CSP.
  name: refundpaymentReference
  type: string
- description: Creditor or CSP requested real-time settlement method. * Refer to Codes and Formats section for more details.
  name: clearingSystem
  type: string
- description: ''
  name: refundAmount
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-account-to-account-commerce-for-creditor-service-providers-refund-payment-schema.json
slug: mastercard-account-to-account-commerce-for-creditor-service-providers-refund-payment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"refundPayment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"refundpaymentReference\": {\n      \"type\": \"string\",\n      \"description\": \"Unique refund payment Reference of the real time settlement method provided by CSP.\"\n    },\n    \"clearingSystem\": {\n      \"type\": \"string\",\n      \"description\": \"Creditor or CSP requested real-time settlement method. * Refer to Codes and Formats section for more details.\"\n    },\n    \"refundAmount\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-account-to-account-commerce-for-creditor-service-providers-refund-payment-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: refundPayment
---
