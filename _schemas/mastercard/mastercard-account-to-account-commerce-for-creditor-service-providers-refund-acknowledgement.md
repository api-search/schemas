---
description: ''
layout: schema
name: RefundAcknowledgement
properties_list:
- description: Unique identifier assigned by Mastercard, to identify the refund request in subsequent transactions or services.
  name: refundRequestLifecycleId
  type: string
- description: Refund Status returned to Mastercard. * Refer to Codes and Formats section for more details.
  name: refundRequestStatus
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-account-to-account-commerce-for-creditor-service-providers-refund-acknowledgement-schema.json
slug: mastercard-account-to-account-commerce-for-creditor-service-providers-refund-acknowledgement
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RefundAcknowledgement\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"refundRequestLifecycleId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier assigned by Mastercard, to identify the refund request in subsequent transactions or services.\"\n    },\n    \"refundRequestStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Refund Status returned to Mastercard. * Refer to Codes and Formats section for more details.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-account-to-account-commerce-for-creditor-service-providers-refund-acknowledgement-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: RefundAcknowledgement
---
