---
description: TransferData schema from Adyen API
layout: schema
name: TransferData
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
- description: The unique identifier of the balance platform.
  name: balancePlatform
  type: string
- description: The list of the latest balance statuses in the transfer.
  name: balances
  type: array
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
- description: The list of events leading up to the current status of the transfer.
  name: events
  type: array
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
- description: 'The sequence number of the transfer notification. The numbers start from 1 and increase with each new notification for a specific transfer. It can help you restore the correct sequence of events even '
  name: sequenceNumber
  type: integer
- description: The result of the transfer. For example, **authorised**, **refused**, or **error**.
  name: status
  type: string
- description: The tracking information for the transfer.
  name: tracking
  type: object
- description: Contains the results of the evaluation of the transaction rules.
  name: transactionRulesResult
  type: object
- description: The type of transfer or transaction. For example, **refund**, **payment**, **internalTransfer**, **bankTransfer**.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfer-webhooks-transfer-data-schema.json
slug: transfer-webhooks-transfer-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-transfer-data-schema.json\",\n  \"title\": \"TransferData\",\n  \"description\": \"TransferData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolder\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The account holder associated with the balance account used in the transfer.\",\n      \"$ref\": \"#/components/schemas/ResourceReference\"\n    },\n    \"amount\": {\n      \"x-addedInVersion\": \"1\",\n      \"description\": \"The amount of the transfer.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"balanceAccount\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"Contains information about the balance account involved in the transfer.\",\n      \"$ref\": \"#/components/schemas/ResourceReference\"\n    },\n\
  \    \"balancePlatform\": {\n      \"description\": \"The unique identifier of the balance platform.\",\n      \"type\": \"string\"\n    },\n    \"balances\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The list of the latest balance statuses in the transfer.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/BalanceMutation\"\n      },\n      \"type\": \"array\"\n    },\n    \"category\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The category of transfer.\\n\\nPossible values:\\n\\n - **bank**: Transfer to a [transfer instrument](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/transferInstruments__resParam_id) or a bank account.\\n\\n- **internal**: Transfer to another [balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/balanceAccounts__resParam_id) within your platform.\\n\\n- **issuedCard**: Transfer initiated by a Adyen-issued card.\\n\\n- **platformPayment**: Fund movements related\
  \ to payments that are acquired for your users.\",\n      \"enum\": [\n        \"bank\",\n        \"internal\",\n        \"issuedCard\",\n        \"platformPayment\"\n      ],\n      \"type\": \"string\"\n    },\n    \"categoryData\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The relevant data according to the transfer category.\",\n      \"oneOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BankCategoryData\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/InternalCategoryData\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/IssuedCard\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/PlatformPayment\"\n        }\n      ]\n    },\n    \"counterparty\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The other party in the transfer.\",\n      \"$ref\": \"#/components/schemas/TransferNotificationCounterParty\"\n    },\n    \"creationDate\": {\n      \"x-addedInVersion\": \"3\",\n\
  \      \"description\": \"The date and time when the event was triggered, in ISO 8601 extended format. For example, **2020-12-18T10:15:30+01:00**.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"x-addedInVersion\": \"1\",\n      \"description\": \"Your description for the transfer. It is used by most banks as the transfer description. We recommend sending a maximum of 140 characters, otherwise the description may be truncated.\\n\\nSupported characters: **[a-z] [A-Z] [0-9] / - ?** **: ( ) . , ' + Space**\\n\\nSupported characters for **regular** and **fast** transfers to a US counterparty: **[a-z] [A-Z] [0-9] & $ % # @** **~ = + - _ ' \\\" ! ?**\",\n      \"type\": \"string\"\n    },\n    \"direction\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The direction of the transfer.\\n\\nPossible values: **incoming**, **outgoing**.\",\n      \"enum\": [\n        \"incoming\",\n        \"outgoing\"\n      ],\n     \
  \ \"type\": \"string\"\n    },\n    \"events\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The list of events leading up to the current status of the transfer.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TransferEvent\"\n      },\n      \"type\": \"array\"\n    },\n    \"id\": {\n      \"description\": \"The ID of the resource.\",\n      \"type\": \"string\"\n    },\n    \"paymentInstrument\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"Contains information about the payment instrument used in the transfer.\",\n      \"$ref\": \"#/components/schemas/PaymentInstrument\"\n    },\n    \"reason\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"Additional information about the status of the transfer.\",\n      \"enum\": [\n        \"amountLimitExceeded\",\n        \"approved\",\n        \"balanceAccountTemporarilyBlockedByTransactionRule\",\n        \"counterpartyAccountBlocked\",\n        \"counterpartyAccountClosed\"\
  ,\n        \"counterpartyAccountNotFound\",\n        \"counterpartyAddressRequired\",\n        \"counterpartyBankTimedOut\",\n        \"counterpartyBankUnavailable\",\n        \"declinedByTransactionRule\",\n        \"error\",\n        \"notEnoughBalance\",\n        \"refusedByCounterpartyBank\",\n        \"routeNotFound\",\n        \"scaFailed\",\n        \"unknown\"\n      ],\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"Your reference for the transfer, used internally within your platform. If you don't provide this in the request, Adyen generates a unique reference.\",\n      \"maxLength\": 80,\n      \"type\": \"string\"\n    },\n    \"referenceForBeneficiary\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \" A reference that is sent to the recipient. This reference is also sent in all webhooks related to the transfer, so you can use it to track statuses for both the source and recipient of funds.\\\
  n\\n Supported characters: **a-z**, **A-Z**, **0-9**. The maximum length depends on the `category`.\\n\\n- **internal**: 80 characters\\n\\n- **bank**: 35 characters when transferring to an IBAN, 15 characters for others.\",\n      \"maxLength\": 80,\n      \"type\": \"string\"\n    },\n    \"sequenceNumber\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The sequence number of the transfer notification. The numbers start from 1 and increase with each new notification for a specific transfer.\\n\\nIt can help you restore the correct sequence of events even if they arrive out of order.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"status\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The result of the transfer.\\n\\n For example, **authorised**, **refused**, or **error**.\",\n      \"enum\": [\n        \"approvalPending\",\n        \"atmWithdrawal\",\n        \"atmWithdrawalReversalPending\",\n        \"atmWithdrawalReversed\"\
  ,\n        \"authAdjustmentAuthorised\",\n        \"authAdjustmentError\",\n        \"authAdjustmentRefused\",\n        \"authorised\",\n        \"bankTransfer\",\n        \"bankTransferPending\",\n        \"booked\",\n        \"bookingPending\",\n        \"cancelled\",\n        \"capturePending\",\n        \"captureReversalPending\",\n        \"captureReversed\",\n        \"captured\",\n        \"capturedExternally\",\n        \"chargeback\",\n        \"chargebackExternally\",\n        \"chargebackPending\",\n        \"chargebackReversalPending\",\n        \"chargebackReversed\",\n        \"credited\",\n        \"depositCorrection\",\n        \"depositCorrectionPending\",\n        \"dispute\",\n        \"disputeClosed\",\n        \"disputeExpired\",\n        \"disputeNeedsReview\",\n        \"error\",\n        \"expired\",\n        \"failed\",\n        \"fee\",\n        \"feePending\",\n        \"internalTransfer\",\n        \"internalTransferPending\",\n        \"invoiceDeduction\",\n\
  \        \"invoiceDeductionPending\",\n        \"manualCorrectionPending\",\n        \"manuallyCorrected\",\n        \"matchedStatement\",\n        \"matchedStatementPending\",\n        \"merchantPayin\",\n        \"merchantPayinPending\",\n        \"merchantPayinReversed\",\n        \"merchantPayinReversedPending\",\n        \"miscCost\",\n        \"miscCostPending\",\n        \"paymentCost\",\n        \"paymentCostPending\",\n        \"received\",\n        \"refundPending\",\n        \"refundReversalPending\",\n        \"refundReversed\",\n        \"refunded\",\n        \"refundedExternally\",\n        \"refused\",\n        \"reserveAdjustment\",\n        \"reserveAdjustmentPending\",\n        \"returned\",\n        \"secondChargeback\",\n        \"secondChargebackPending\",\n        \"undefined\"\n      ],\n      \"type\": \"string\"\n    },\n    \"tracking\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The tracking information for the transfer.\",\n      \"$ref\"\
  : \"#/components/schemas/TransferNotificationTransferTracking\"\n    },\n    \"transactionRulesResult\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"Contains the results of the evaluation of the transaction rules.\",\n      \"$ref\": \"#/components/schemas/TransactionRulesResult\"\n    },\n    \"type\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The type of transfer or transaction. For example, **refund**, **payment**, **internalTransfer**, **bankTransfer**.\",\n      \"enum\": [\n        \"atmWithdrawal\",\n        \"atmWithdrawalReversal\",\n        \"balanceAdjustment\",\n        \"balanceMigration\",\n        \"balanceRollover\",\n        \"bankTransfer\",\n        \"capture\",\n        \"captureReversal\",\n        \"cardTransfer\",\n        \"cashOutFee\",\n        \"cashOutFunding\",\n        \"cashOutInstruction\",\n        \"chargeback\",\n        \"chargebackCorrection\",\n        \"chargebackReversal\",\n        \"chargebackReversalCorrection\"\
  ,\n        \"depositCorrection\",\n        \"fee\",\n        \"grant\",\n        \"installment\",\n        \"installmentReversal\",\n        \"internalTransfer\",\n        \"invoiceDeduction\",\n        \"leftover\",\n        \"manualCorrection\",\n        \"miscCost\",\n        \"payment\",\n        \"paymentCost\",\n        \"refund\",\n        \"refundReversal\",\n        \"repayment\",\n        \"reserveAdjustment\",\n        \"secondChargeback\",\n        \"secondChargebackCorrection\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"category\",\n    \"amount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-transfer-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransferData
---
