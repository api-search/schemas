---
description: TransferEvent schema from Adyen API
layout: schema
name: TransferEvent
properties_list:
- description: The amount adjustments in this transfer.
  name: amountAdjustments
  type: array
- description: The date when the transfer request was sent.
  name: bookingDate
  type: string
- description: The unique identifier of the transfer event.
  name: id
  type: string
- description: The list of the balance mutation per event.
  name: mutations
  type: array
- description: The amount in the original currency.
  name: originalAmount
  type: object
- description: The reason for the transfer status.
  name: reason
  type: string
- description: The status of the transfer event.
  name: status
  type: string
- description: The id of the transaction that is related to this accounting event. Only sent for events of type **accounting** where the balance changes.
  name: transactionId
  type: string
- description: 'The type of the transfer event. Possible values: **accounting**, **tracking**.'
  name: type
  type: string
- description: The date when the tracking status was updated.
  name: updateDate
  type: string
- description: A future date, when the funds are expected to be deducted from or credited to the balance account.
  name: valueDate
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounting-notifications-transfer-event-schema.json
slug: accounting-notifications-transfer-event
source_filename: accounting-notifications-transfer-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-transfer-event-schema.json\",\n  \"title\": \"TransferEvent\",\n  \"description\": \"TransferEvent schema from Adyen API\",\n  \"properties\": {\n    \"amountAdjustments\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The amount adjustments in this transfer.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AmountAdjustment\"\n      },\n      \"type\": \"array\"\n    },\n    \"bookingDate\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The date when the transfer request was sent.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The unique identifier of the transfer event.\",\n      \"type\": \"string\"\n    },\n    \"mutations\": {\n  \
  \    \"x-addedInVersion\": \"3\",\n      \"description\": \"The list of the balance mutation per event.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/BalanceMutation\"\n      },\n      \"type\": \"array\"\n    },\n    \"originalAmount\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The amount in the original currency.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"reason\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The reason for the transfer status.\",\n      \"enum\": [\n        \"amountLimitExceded\",\n        \"approved\",\n        \"counterpartyAccountBlocked\",\n        \"counterpartyAccountClosed\",\n        \"counterpartyAccountNotFound\",\n        \"counterpartyAddressRequired\",\n        \"counterpartyBankTimedOut\",\n        \"counterpartyBankUnavailable\",\n        \"error\",\n        \"notEnoughBalance\",\n        \"refusedByCounterpartyBank\",\n        \"routeNotFound\",\n        \"unknown\"\n\
  \      ],\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The status of the transfer event.\",\n      \"enum\": [\n        \"atmWithdrawal\",\n        \"atmWithdrawalReversalPending\",\n        \"atmWithdrawalReversed\",\n        \"authAdjustmentAuthorised\",\n        \"authAdjustmentError\",\n        \"authAdjustmentRefused\",\n        \"authorised\",\n        \"bankTransfer\",\n        \"bankTransferPending\",\n        \"booked\",\n        \"bookingPending\",\n        \"cancelled\",\n        \"capturePending\",\n        \"captureReversalPending\",\n        \"captureReversed\",\n        \"captured\",\n        \"chargeback\",\n        \"chargebackPending\",\n        \"chargebackReversalPending\",\n        \"chargebackReversed\",\n        \"credited\",\n        \"depositCorrection\",\n        \"depositCorrectionPending\",\n        \"dispute\",\n        \"disputeClosed\",\n        \"disputeExpired\",\n        \"disputeNeedsReview\"\
  ,\n        \"error\",\n        \"expired\",\n        \"failed\",\n        \"fee\",\n        \"feePending\",\n        \"internalTransfer\",\n        \"internalTransferPending\",\n        \"invoiceDeduction\",\n        \"invoiceDeductionPending\",\n        \"manualCorrectionPending\",\n        \"manuallyCorrected\",\n        \"matchedStatement\",\n        \"matchedStatementPending\",\n        \"merchantPayin\",\n        \"merchantPayinPending\",\n        \"merchantPayinReversed\",\n        \"merchantPayinReversedPending\",\n        \"miscCost\",\n        \"miscCostPending\",\n        \"paymentCost\",\n        \"paymentCostPending\",\n        \"received\",\n        \"refundPending\",\n        \"refundReversalPending\",\n        \"refundReversed\",\n        \"refunded\",\n        \"refused\",\n        \"reserveAdjustment\",\n        \"reserveAdjustmentPending\",\n        \"returned\",\n        \"secondChargeback\",\n        \"secondChargebackPending\",\n        \"undefined\"\n      ],\n  \
  \    \"type\": \"string\"\n    },\n    \"transactionId\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The id of the transaction that is related to this accounting event. Only sent for events of type **accounting** where the balance changes.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The type of the transfer event. Possible values: **accounting**, **tracking**.\",\n      \"enum\": [\n        \"accounting\",\n        \"tracking\"\n      ],\n      \"type\": \"string\"\n    },\n    \"updateDate\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The date when the tracking status was updated.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"valueDate\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"A future date, when the funds are expected to be deducted from or credited to the balance account.\",\n      \"format\": \"date-time\",\n\
  \      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-transfer-event-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransferEvent
---
