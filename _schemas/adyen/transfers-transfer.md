---
description: Transfer schema from Adyen API
layout: schema
name: Transfer
properties_list:
- description: The account holder associated with the balance account used in the transfer.
  name: accountHolder
  type: object
- description: The amount of the transfer.
  name: amount
  type: object
- description: Contains information about the balance account involved in the transfer.
  name: balanceAccount
  type: object
- description: 'The category of transfer. Possible values: - **bank**: Transfer to a [transfer instrument](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/transferInstruments__resParam_id) or a bank acc'
  name: category
  type: string
- description: The relevant data according to the transfer category.
  name: categoryData
  type: object
- description: The other party in the transfer.
  name: counterparty
  type: object
- description: The date and time when the event was triggered, in ISO 8601 extended format. For example, **2020-12-18T10:15:30+01:00**.
  name: creationDate
  type: string
- description: Your description for the transfer. It is used by most banks as the transfer description. We recommend sending a maximum of 140 characters, otherwise the description may be truncated. Supported charact
  name: description
  type: string
- description: 'The direction of the transfer. Possible values: **incoming**, **outgoing**.'
  name: direction
  type: string
- description: The ID of the resource.
  name: id
  type: string
- description: Contains information about the payment instrument used in the transfer.
  name: paymentInstrument
  type: object
- description: Additional information about the status of the transfer.
  name: reason
  type: string
- description: Your reference for the transfer, used internally within your platform. If you don't provide this in the request, Adyen generates a unique reference.
  name: reference
  type: string
- description: A reference that is sent to the recipient. This reference is also sent in all webhooks related to the transfer, so you can use it to track statuses for both the source and recipient of funds. Supporte
  name: referenceForBeneficiary
  type: string
- description: The result of the transfer. For example, **authorised**, **refused**, or **error**.
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-transfer-schema.json
slug: transfers-transfer
source_filename: transfers-transfer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-transfer-schema.json\",\n  \"title\": \"Transfer\",\n  \"description\": \"Transfer schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolder\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The account holder associated with the balance account used in the transfer.\",\n      \"$ref\": \"#/components/schemas/ResourceReference\"\n    },\n    \"amount\": {\n      \"x-addedInVersion\": \"1\",\n      \"description\": \"The amount of the transfer.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"balanceAccount\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"Contains information about the balance account involved in the transfer.\",\n      \"$ref\": \"#/components/schemas/ResourceReference\"\n    },\n    \"category\": {\n\
  \      \"x-addedInVersion\": \"3\",\n      \"description\": \"The category of transfer.\\n\\nPossible values:\\n\\n - **bank**: Transfer to a [transfer instrument](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/transferInstruments__resParam_id) or a bank account.\\n\\n- **internal**: Transfer to another [balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/balanceAccounts__resParam_id) within your platform.\\n\\n- **issuedCard**: Transfer initiated by a Adyen-issued card.\\n\\n- **platformPayment**: Fund movements related to payments that are acquired for your users.\",\n      \"enum\": [\n        \"bank\",\n        \"internal\",\n        \"issuedCard\",\n        \"platformPayment\"\n      ],\n      \"type\": \"string\"\n    },\n    \"categoryData\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The relevant data according to the transfer category.\",\n      \"oneOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BankCategoryData\"\
  \n        },\n        {\n          \"$ref\": \"#/components/schemas/InternalCategoryData\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/IssuedCard\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/PlatformPayment\"\n        }\n      ]\n    },\n    \"counterparty\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The other party in the transfer.\",\n      \"$ref\": \"#/components/schemas/CounterpartyV3\"\n    },\n    \"creationDate\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The date and time when the event was triggered, in ISO 8601 extended format. For example, **2020-12-18T10:15:30+01:00**.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"x-addedInVersion\": \"1\",\n      \"description\": \"Your description for the transfer. It is used by most banks as the transfer description. We recommend sending a maximum of 140 characters, otherwise the description\
  \ may be truncated.\\n\\nSupported characters: **[a-z] [A-Z] [0-9] / - ?** **: ( ) . , ' + Space**\\n\\nSupported characters for **regular** and **fast** transfers to a US counterparty: **[a-z] [A-Z] [0-9] & $ % # @** **~ = + - _ ' \\\" ! ?**\",\n      \"type\": \"string\"\n    },\n    \"direction\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The direction of the transfer.\\n\\nPossible values: **incoming**, **outgoing**.\",\n      \"enum\": [\n        \"incoming\",\n        \"outgoing\"\n      ],\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The ID of the resource.\",\n      \"type\": \"string\"\n    },\n    \"paymentInstrument\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"Contains information about the payment instrument used in the transfer.\",\n      \"$ref\": \"#/components/schemas/PaymentInstrument\"\n    },\n    \"reason\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"Additional information\
  \ about the status of the transfer.\",\n      \"enum\": [\n        \"amountLimitExceeded\",\n        \"approved\",\n        \"balanceAccountTemporarilyBlockedByTransactionRule\",\n        \"counterpartyAccountBlocked\",\n        \"counterpartyAccountClosed\",\n        \"counterpartyAccountNotFound\",\n        \"counterpartyAddressRequired\",\n        \"counterpartyBankTimedOut\",\n        \"counterpartyBankUnavailable\",\n        \"declinedByTransactionRule\",\n        \"error\",\n        \"notEnoughBalance\",\n        \"refusedByCounterpartyBank\",\n        \"routeNotFound\",\n        \"scaFailed\",\n        \"unknown\"\n      ],\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"Your reference for the transfer, used internally within your platform. If you don't provide this in the request, Adyen generates a unique reference.\",\n      \"maxLength\": 80,\n      \"type\": \"string\"\n    },\n    \"referenceForBeneficiary\"\
  : {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \" A reference that is sent to the recipient. This reference is also sent in all webhooks related to the transfer, so you can use it to track statuses for both the source and recipient of funds.\\n\\n Supported characters: **a-z**, **A-Z**, **0-9**. The maximum length depends on the `category`.\\n\\n- **internal**: 80 characters\\n\\n- **bank**: 35 characters when transferring to an IBAN, 15 characters for others.\",\n      \"maxLength\": 80,\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The result of the transfer.\\n\\n For example, **authorised**, **refused**, or **error**.\",\n      \"enum\": [\n        \"approvalPending\",\n        \"atmWithdrawal\",\n        \"atmWithdrawalReversalPending\",\n        \"atmWithdrawalReversed\",\n        \"authAdjustmentAuthorised\",\n        \"authAdjustmentError\",\n        \"authAdjustmentRefused\",\n        \"authorised\"\
  ,\n        \"bankTransfer\",\n        \"bankTransferPending\",\n        \"booked\",\n        \"bookingPending\",\n        \"cancelled\",\n        \"capturePending\",\n        \"captureReversalPending\",\n        \"captureReversed\",\n        \"captured\",\n        \"capturedExternally\",\n        \"chargeback\",\n        \"chargebackExternally\",\n        \"chargebackPending\",\n        \"chargebackReversalPending\",\n        \"chargebackReversed\",\n        \"credited\",\n        \"depositCorrection\",\n        \"depositCorrectionPending\",\n        \"dispute\",\n        \"disputeClosed\",\n        \"disputeExpired\",\n        \"disputeNeedsReview\",\n        \"error\",\n        \"expired\",\n        \"failed\",\n        \"fee\",\n        \"feePending\",\n        \"internalTransfer\",\n        \"internalTransferPending\",\n        \"invoiceDeduction\",\n        \"invoiceDeductionPending\",\n        \"manualCorrectionPending\",\n        \"manuallyCorrected\",\n        \"matchedStatement\"\
  ,\n        \"matchedStatementPending\",\n        \"merchantPayin\",\n        \"merchantPayinPending\",\n        \"merchantPayinReversed\",\n        \"merchantPayinReversedPending\",\n        \"miscCost\",\n        \"miscCostPending\",\n        \"paymentCost\",\n        \"paymentCostPending\",\n        \"received\",\n        \"refundPending\",\n        \"refundReversalPending\",\n        \"refundReversed\",\n        \"refunded\",\n        \"refundedExternally\",\n        \"refused\",\n        \"reserveAdjustment\",\n        \"reserveAdjustmentPending\",\n        \"returned\",\n        \"secondChargeback\",\n        \"secondChargebackPending\",\n        \"undefined\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"counterparty\",\n    \"status\",\n    \"category\",\n    \"amount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-transfer-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Transfer
---
