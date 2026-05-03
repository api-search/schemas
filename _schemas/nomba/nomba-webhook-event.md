---
description: Schema for validating Nomba webhook event payloads delivered to merchant endpoints when subscribed events occur.
layout: schema
name: Nomba Webhook Event
properties_list:
- description: The type of event that triggered the webhook notification.
  name: event_type
  type: string
- description: A unique identifier for this webhook delivery request, useful for deduplication.
  name: requestId
  type: string
- description: The event payload containing merchant, terminal, and transaction details.
  name: data
  type: object
provider_name: Nomba
provider_slug: nomba
schema_file: json-schema/nomba-webhook-event-schema.json
slug: nomba-webhook-event
source_filename: nomba-webhook-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.nomba.com/schemas/nomba/webhook-event.json\",\n  \"title\": \"Nomba Webhook Event\",\n  \"description\": \"Schema for validating Nomba webhook event payloads delivered to merchant endpoints when subscribed events occur.\",\n  \"type\": \"object\",\n  \"required\": [\"event_type\", \"requestId\", \"data\"],\n  \"properties\": {\n    \"event_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of event that triggered the webhook notification.\",\n      \"enum\": [\n        \"payment_success\",\n        \"payment_failed\",\n        \"payout_success\",\n        \"payout_failed\",\n        \"order_success\",\n        \"payment_reversal\",\n        \"payout_refund\"\n      ]\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"A unique identifier for this webhook delivery request, useful for deduplication.\"\
  \n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"The event payload containing merchant, terminal, and transaction details.\",\n      \"required\": [\"merchant\", \"transaction\"],\n      \"properties\": {\n        \"merchant\": {\n          \"$ref\": \"#/$defs/Merchant\"\n        },\n        \"terminal\": {\n          \"$ref\": \"#/$defs/Terminal\"\n        },\n        \"transaction\": {\n          \"$ref\": \"#/$defs/Transaction\"\n        },\n        \"order\": {\n          \"$ref\": \"#/$defs/Order\"\n        },\n        \"originalTransactionId\": {\n          \"type\": \"string\",\n          \"description\": \"The transaction ID of the original payment or payout for reversal and refund events.\"\n        },\n        \"error\": {\n          \"type\": \"string\",\n          \"description\": \"A description of why the payment or payout failed, present on failure events.\"\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"Merchant\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"Merchant account information associated with the event.\",\n      \"properties\": {\n        \"walletId\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the merchant wallet.\"\n        },\n        \"walletBalance\": {\n          \"type\": \"number\",\n          \"description\": \"The current wallet balance after the event occurred.\"\n        },\n        \"userId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the merchant user.\"\n        }\n      }\n    },\n    \"Terminal\": {\n      \"type\": \"object\",\n      \"description\": \"POS terminal information, populated for terminal-based transactions.\",\n      \"properties\": {\n        \"terminalId\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the POS terminal.\"\n        },\n        \"serialNumber\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"The serial number of the POS terminal hardware.\"\n        }\n      }\n    },\n    \"Transaction\": {\n      \"type\": \"object\",\n      \"description\": \"Transaction details for the event.\",\n      \"properties\": {\n        \"transactionId\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the transaction.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of transaction, such as vact_transfer for virtual account transfers.\"\n        },\n        \"aliasAccountNumber\": {\n          \"type\": \"string\",\n          \"description\": \"The alias account number associated with the transaction.\"\n        },\n        \"amount\": {\n          \"type\": \"number\",\n          \"description\": \"The transaction amount.\"\n        },\n        \"fee\": {\n          \"type\": \"number\",\n          \"description\": \"The fee charged for the transaction.\"\n    \
  \    },\n        \"sessionId\": {\n          \"type\": \"string\",\n          \"description\": \"The session identifier for the transaction.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The status of the transaction.\",\n          \"enum\": [\"successful\", \"failed\", \"reversed\", \"refunded\"]\n        }\n      }\n    },\n    \"Order\": {\n      \"type\": \"object\",\n      \"description\": \"Checkout order information, present on order_success events.\",\n      \"properties\": {\n        \"orderReference\": {\n          \"type\": \"string\",\n          \"description\": \"The unique reference for the checkout order.\"\n        },\n        \"amount\": {\n          \"type\": \"number\",\n          \"description\": \"The order amount.\"\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"description\": \"The currency of the order.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/json-schema/nomba-webhook-event-schema.json
tags:
- Payments
- Fintech
- Banking
- Transfers
- Virtual Accounts
- Checkout
- Cross-Border Payments
- Cards
title: Nomba Webhook Event
---
