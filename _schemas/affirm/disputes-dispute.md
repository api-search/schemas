---
description: Represents a payment dispute filed by a customer against an Affirm transaction, including its current status, reason, and any evidence submitted by the merchant.
layout: schema
name: Dispute
properties_list:
- description: Unique identifier for this dispute.
  name: id
  type: string
- description: The identifier of the Affirm transaction being disputed.
  name: transaction_id
  type: string
- description: The identifier of the charge associated with this dispute.
  name: charge_id
  type: string
- description: Current status of the dispute.
  name: status
  type: string
- description: Standardized reason code categorizing the nature of the dispute (e.g., item_not_received, item_not_as_described, unauthorized).
  name: reason_code
  type: string
- description: The disputed amount in cents.
  name: amount
  type: integer
- description: ISO 4217 currency code for the disputed amount.
  name: currency
  type: string
- description: Timestamp when this dispute was created, in RFC 3339 format.
  name: created
  type: string
- description: Deadline by which the merchant must submit evidence to contest this dispute, in RFC 3339 format.
  name: evidence_due_by
  type: string
- description: Timestamp when this dispute was closed, if applicable.
  name: closed_at
  type: string
- description: Final outcome of the dispute after review. Only set when status is won or lost.
  name: outcome
  type: string
- description: List of evidence items submitted by the merchant for this dispute.
  name: evidence
  type: array
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/disputes-dispute-schema.json
slug: disputes-dispute
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/disputes-dispute-schema.json\",\n  \"title\": \"Dispute\",\n  \"description\": \"Represents a payment dispute filed by a customer against an Affirm transaction, including its current status, reason, and any evidence submitted by the merchant.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this dispute.\",\n      \"example\": \"500123\"\n    },\n    \"transaction_id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the Affirm transaction being disputed.\",\n      \"example\": \"500123\"\n    },\n    \"charge_id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the charge associated with this dispute.\",\n      \"example\": \"500123\"\n    },\n    \"status\": {\n  \
  \    \"type\": \"string\",\n      \"description\": \"Current status of the dispute.\",\n      \"enum\": [\n        \"open\",\n        \"closed\",\n        \"won\",\n        \"lost\"\n      ],\n      \"example\": \"open\"\n    },\n    \"reason_code\": {\n      \"type\": \"string\",\n      \"description\": \"Standardized reason code categorizing the nature of the dispute (e.g., item_not_received, item_not_as_described, unauthorized).\",\n      \"example\": \"example_value\"\n    },\n    \"amount\": {\n      \"type\": \"integer\",\n      \"description\": \"The disputed amount in cents.\",\n      \"example\": 1\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code for the disputed amount.\",\n      \"example\": \"USD\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when this dispute was created, in RFC 3339 format.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\
  \n    },\n    \"evidence_due_by\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Deadline by which the merchant must submit evidence to contest this dispute, in RFC 3339 format.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"closed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"description\": \"Timestamp when this dispute was closed, if applicable.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"outcome\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Final outcome of the dispute after review. Only set when status is won or lost.\",\n      \"enum\": [\n        \"merchant_won\",\n        \"merchant_lost\"\n      ],\n      \"example\": \"merchant_won\"\n    },\n    \"evidence\": {\n      \"type\": \"array\",\n      \"description\": \"List of evidence items submitted by the merchant for this dispute.\",\n      \"items\"\
  : {\n        \"$ref\": \"#/components/schemas/EvidenceItem\"\n      },\n      \"example\": [\n        \"example_value\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/disputes-dispute-schema.json
tags: []
title: Dispute
---
