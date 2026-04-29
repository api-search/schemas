---
description: ''
layout: schema
name: Status
properties_list:
- description: Status of the transaction. * Refer to Codes and Formats section for more details.
  name: transactionStatus
  type: string
- description: Reason for declined transaction. * Refer to Codes and Formats section for more details.
  name: transactionStatusReason
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-debtor-service-provider-resources-status-schema.json
slug: mastercard-debtor-service-provider-resources-status
source_filename: mastercard-debtor-service-provider-resources-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Status\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactionStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the transaction. * Refer to Codes and Formats section for more details.\"\n    },\n    \"transactionStatusReason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for declined transaction. * Refer to Codes and Formats section for more details.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-debtor-service-provider-resources-status-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Status
---
