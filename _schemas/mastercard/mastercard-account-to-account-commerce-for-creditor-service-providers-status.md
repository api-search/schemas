---
description: ''
layout: schema
name: status
properties_list:
- description: Status of the transaction. * Refer to Codes and Formats section for more details.
  name: refundStatus
  type: string
- description: Reason for declined transaction. * Refer to Codes and Formats section for more details.
  name: refundStatusReason
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-account-to-account-commerce-for-creditor-service-providers-status-schema.json
slug: mastercard-account-to-account-commerce-for-creditor-service-providers-status
source_filename: mastercard-account-to-account-commerce-for-creditor-service-providers-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"status\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"refundStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the transaction. * Refer to Codes and Formats section for more details.\"\n    },\n    \"refundStatusReason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for declined transaction. * Refer to Codes and Formats section for more details.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-account-to-account-commerce-for-creditor-service-providers-status-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: status
---
