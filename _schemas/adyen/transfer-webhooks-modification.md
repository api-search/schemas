---
description: Modification schema from Adyen API
layout: schema
name: Modification
properties_list:
- description: The direction of the money movement.
  name: direction
  type: string
- description: Our reference for the modification.
  name: id
  type: string
- description: Your reference for the modification, used internally within your platform.
  name: reference
  type: string
- description: The status of the transfer event.
  name: status
  type: string
- description: The type of transfer modification.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfer-webhooks-modification-schema.json
slug: transfer-webhooks-modification
source_filename: transfer-webhooks-modification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-modification-schema.json\",\n  \"title\": \"Modification\",\n  \"description\": \"Modification schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"direction\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The direction of the money movement.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"Our reference for the modification.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"Your reference for the modification, used internally within your platform.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The status of the transfer event.\",\n      \"enum\"\
  : [\n        \"approvalPending\",\n        \"atmWithdrawal\",\n        \"atmWithdrawalReversalPending\",\n        \"atmWithdrawalReversed\",\n        \"authAdjustmentAuthorised\",\n        \"authAdjustmentError\",\n        \"authAdjustmentRefused\",\n        \"authorised\",\n        \"bankTransfer\",\n        \"bankTransferPending\",\n        \"booked\",\n        \"bookingPending\",\n        \"cancelled\",\n        \"capturePending\",\n        \"captureReversalPending\",\n        \"captureReversed\",\n        \"captured\",\n        \"capturedExternally\",\n        \"chargeback\",\n        \"chargebackExternally\",\n        \"chargebackPending\",\n        \"chargebackReversalPending\",\n        \"chargebackReversed\",\n        \"credited\",\n        \"depositCorrection\",\n        \"depositCorrectionPending\",\n        \"dispute\",\n        \"disputeClosed\",\n        \"disputeExpired\",\n        \"disputeNeedsReview\",\n        \"error\",\n        \"expired\",\n        \"failed\",\n  \
  \      \"fee\",\n        \"feePending\",\n        \"internalTransfer\",\n        \"internalTransferPending\",\n        \"invoiceDeduction\",\n        \"invoiceDeductionPending\",\n        \"manualCorrectionPending\",\n        \"manuallyCorrected\",\n        \"matchedStatement\",\n        \"matchedStatementPending\",\n        \"merchantPayin\",\n        \"merchantPayinPending\",\n        \"merchantPayinReversed\",\n        \"merchantPayinReversedPending\",\n        \"miscCost\",\n        \"miscCostPending\",\n        \"paymentCost\",\n        \"paymentCostPending\",\n        \"received\",\n        \"refundPending\",\n        \"refundReversalPending\",\n        \"refundReversed\",\n        \"refunded\",\n        \"refundedExternally\",\n        \"refused\",\n        \"reserveAdjustment\",\n        \"reserveAdjustmentPending\",\n        \"returned\",\n        \"secondChargeback\",\n        \"secondChargebackPending\",\n        \"undefined\"\n      ],\n      \"type\": \"string\"\n    },\n\
  \    \"type\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The type of transfer modification.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-modification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Modification
---
