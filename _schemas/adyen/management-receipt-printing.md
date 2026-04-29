---
description: ReceiptPrinting schema from Adyen API
layout: schema
name: ReceiptPrinting
properties_list:
- description: Print a merchant receipt when the payment is approved.
  name: merchantApproved
  type: boolean
- description: Print a merchant receipt when the transaction is cancelled.
  name: merchantCancelled
  type: boolean
- description: Print a merchant receipt when capturing the payment is approved.
  name: merchantCaptureApproved
  type: boolean
- description: Print a merchant receipt when capturing the payment is refused.
  name: merchantCaptureRefused
  type: boolean
- description: Print a merchant receipt when the refund is approved.
  name: merchantRefundApproved
  type: boolean
- description: Print a merchant receipt when the refund is refused.
  name: merchantRefundRefused
  type: boolean
- description: Print a merchant receipt when the payment is refused.
  name: merchantRefused
  type: boolean
- description: Print a merchant receipt when a previous transaction is voided.
  name: merchantVoid
  type: boolean
- description: Print a shopper receipt when the payment is approved.
  name: shopperApproved
  type: boolean
- description: Print a shopper receipt when the transaction is cancelled.
  name: shopperCancelled
  type: boolean
- description: Print a shopper receipt when capturing the payment is approved.
  name: shopperCaptureApproved
  type: boolean
- description: Print a shopper receipt when capturing the payment is refused.
  name: shopperCaptureRefused
  type: boolean
- description: Print a shopper receipt when the refund is approved.
  name: shopperRefundApproved
  type: boolean
- description: Print a shopper receipt when the refund is refused.
  name: shopperRefundRefused
  type: boolean
- description: Print a shopper receipt when the payment is refused.
  name: shopperRefused
  type: boolean
- description: Print a shopper receipt when a previous transaction is voided.
  name: shopperVoid
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-receipt-printing-schema.json
slug: management-receipt-printing
source_filename: management-receipt-printing-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-receipt-printing-schema.json\",\n  \"title\": \"ReceiptPrinting\",\n  \"description\": \"ReceiptPrinting schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"merchantApproved\": {\n      \"description\": \"Print a merchant receipt when the payment is approved.\",\n      \"type\": \"boolean\"\n    },\n    \"merchantCancelled\": {\n      \"description\": \"Print a merchant receipt when the transaction is cancelled.\",\n      \"type\": \"boolean\"\n    },\n    \"merchantCaptureApproved\": {\n      \"description\": \"Print a merchant receipt when capturing the payment is approved.\",\n      \"type\": \"boolean\"\n    },\n    \"merchantCaptureRefused\": {\n      \"description\": \"Print a merchant receipt when capturing the payment is refused.\",\n      \"type\": \"boolean\"\n    },\n\
  \    \"merchantRefundApproved\": {\n      \"description\": \"Print a merchant receipt when the refund is approved.\",\n      \"type\": \"boolean\"\n    },\n    \"merchantRefundRefused\": {\n      \"description\": \"Print a merchant receipt when the refund is refused.\",\n      \"type\": \"boolean\"\n    },\n    \"merchantRefused\": {\n      \"description\": \"Print a merchant receipt when the payment is refused.\",\n      \"type\": \"boolean\"\n    },\n    \"merchantVoid\": {\n      \"description\": \"Print a merchant receipt when a previous transaction is voided.\",\n      \"type\": \"boolean\"\n    },\n    \"shopperApproved\": {\n      \"description\": \"Print a shopper receipt when the payment is approved.\",\n      \"type\": \"boolean\"\n    },\n    \"shopperCancelled\": {\n      \"description\": \"Print a shopper receipt when the transaction is cancelled.\",\n      \"type\": \"boolean\"\n    },\n    \"shopperCaptureApproved\": {\n      \"description\": \"Print a shopper receipt when\
  \ capturing the payment is approved.\",\n      \"type\": \"boolean\"\n    },\n    \"shopperCaptureRefused\": {\n      \"description\": \"Print a shopper receipt when capturing the payment is refused.\",\n      \"type\": \"boolean\"\n    },\n    \"shopperRefundApproved\": {\n      \"description\": \"Print a shopper receipt when the refund is approved.\",\n      \"type\": \"boolean\"\n    },\n    \"shopperRefundRefused\": {\n      \"description\": \"Print a shopper receipt when the refund is refused.\",\n      \"type\": \"boolean\"\n    },\n    \"shopperRefused\": {\n      \"description\": \"Print a shopper receipt when the payment is refused.\",\n      \"type\": \"boolean\"\n    },\n    \"shopperVoid\": {\n      \"description\": \"Print a shopper receipt when a previous transaction is voided.\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-receipt-printing-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ReceiptPrinting
---
