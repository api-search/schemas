---
description: TransferNotificationData schema from Adyen API
layout: schema
name: TransferNotificationData
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
- description: The unique identifier of the source [balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/balanceAccounts__resParam_id).
  name: balanceAccountId
  type: string
- description: The list of the latest balance statuses in the transfer.
  name: balances
  type: array
- description: 'The type of transfer. Possible values: - **bank**: Transfer to a [transfer instrument](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/transferInstruments__resParam_id) or a bank account'
  name: category
  type: string
- description: The other party in the transfer.
  name: counterparty
  type: object
- description: A human-readable description for the transfer. You can use alphanumeric characters and hyphens. We recommend sending a maximum of 140 characters, otherwise the description may be truncated.
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
- description: The capture's merchant reference included in the transfer.
  name: modificationMerchantReference
  type: string
- description: The capture reference included in the transfer.
  name: modificationPspReference
  type: string
- description: 'Indicates the method used for entering the PAN to initiate a transaction. Possible values: **manual**, **chip**, **magstripe**, **contactless**, **cof**, **ecommerce**, **token**.'
  name: panEntryMode
  type: string
- description: Contains information about the payment instrument used in the transfer.
  name: paymentInstrument
  type: object
- description: The unique identifier of the source [payment instrument](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/paymentInstruments__resParam_id).
  name: paymentInstrumentId
  type: string
- description: The payment's merchant reference included in the transfer.
  name: paymentMerchantReference
  type: string
- description: 'The priority for the bank transfer. This sets the speed at which the transfer is sent and the fees that you have to pay. Required for transfers with `category` **bank**. Possible values: * **regular**'
  name: priority
  type: string
- description: Contains information about how the payment was processed. For example, **ecommerce** for online or **pos** for in-person payments.
  name: processingType
  type: string
- description: The payment reference included in the transfer.
  name: pspPaymentReference
  type: string
- description: Additional information about the status of the transfer.
  name: reason
  type: string
- description: Your reference for the transfer, used internally within your platform. If you don't provide this in the request, Adyen generates a unique reference.
  name: reference
  type: string
- description: A reference that is sent to the recipient. This reference is also sent in all notification webhooks related to the transfer, so you can use it to track statuses for both the source and recipient of fu
  name: referenceForBeneficiary
  type: string
- description: If you are using relayed authorisation, this object contains information from the relayed authorisation response from your server.
  name: relayedAuthorisationData
  type: object
- description: 'The sequence number of the transfer notification. The numbers start from 1 and increase with each new notification for a specific transfer. It can help you restore the correct sequence of events even '
  name: sequenceNumber
  type: integer
- description: The result of the transfer. For example, **authorised**, **refused**, or **error**.
  name: status
  type: string
- description: The tracking information for the transfer.
  name: tracking
  type: object
- description: The ID of the transaction that is created based on the transfer.
  name: transactionId
  type: string
- description: Contains the results of the evaluation of the transaction rules.
  name: transactionRulesResult
  type: object
- description: The type of transfer or transaction. For example, **refund**, **payment**, **internalTransfer**, **bankTransfer**.
  name: type
  type: string
- description: The evaluation of the validation facts. See [validation checks](https://docs.adyen.com/issuing/validation-checks) for more information.
  name: validationFacts
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounting-notifications-transfer-notification-data-schema.json
slug: accounting-notifications-transfer-notification-data
source_filename: accounting-notifications-transfer-notification-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-transfer-notification-data-schema.json\",\n  \"title\": \"TransferNotificationData\",\n  \"description\": \"TransferNotificationData schema from Adyen API\",\n  \"properties\": {\n    \"accountHolder\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The account holder associated with the balance account used in the transfer.\",\n      \"$ref\": \"#/components/schemas/ResourceReference\"\n    },\n    \"amount\": {\n      \"x-addedInVersion\": \"1\",\n      \"description\": \"The amount of the transfer.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"balanceAccount\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"Contains information about the balance account involved in the transfer.\",\n      \"$ref\": \"#/components/schemas/ResourceReference\"\
  \n    },\n    \"balanceAccountId\": {\n      \"x-addedInVersion\": \"3\",\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"3\",\n      \"x-deprecatedMessage\": \"Use the [id](https://docs.adyen.com/api-explorer/accounting-webhooks/latest/post/balancePlatform.transfer.created#request-data-balanceAccount-id) in the `balanceAccount` object instead.\",\n      \"description\": \"The unique identifier of the source [balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/balanceAccounts__resParam_id).\",\n      \"type\": \"string\"\n    },\n    \"balances\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The list of the latest balance statuses in the transfer.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/BalanceMutation\"\n      },\n      \"type\": \"array\"\n    },\n    \"category\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The type of transfer.\\n\\nPossible values:\\n\\n - **bank**: Transfer\
  \ to a [transfer instrument](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/transferInstruments__resParam_id) or a bank account.\\n\\n- **internal**: Transfer to another [balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/balanceAccounts__resParam_id) within your platform.\\n\\n- **issuedCard**: Transfer initiated by a Adyen-issued card.\\n\\n- **platformPayment**: Fund movements related to payments that are acquired for your users.\",\n      \"enum\": [\n        \"bank\",\n        \"internal\",\n        \"issuedCard\",\n        \"platformPayment\"\n      ],\n      \"type\": \"string\"\n    },\n    \"counterparty\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The other party in the transfer.\",\n      \"$ref\": \"#/components/schemas/CounterpartyV3\"\n    },\n    \"description\": {\n      \"x-addedInVersion\": \"1\",\n      \"description\": \"A human-readable description for the transfer. You can use alphanumeric characters\
  \ and hyphens. We recommend sending a maximum of 140 characters, otherwise the description may be truncated.\",\n      \"type\": \"string\"\n    },\n    \"direction\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The direction of the transfer.\\n\\nPossible values: **incoming**, **outgoing**.\",\n      \"enum\": [\n        \"incoming\",\n        \"outgoing\"\n      ],\n      \"type\": \"string\"\n    },\n    \"events\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The list of events leading up to the current status of the transfer.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TransferEvent\"\n      },\n      \"type\": \"array\"\n    },\n    \"id\": {\n      \"description\": \"The ID of the resource.\",\n      \"type\": \"string\"\n    },\n    \"modificationMerchantReference\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The capture's merchant reference included in the transfer.\",\n      \"type\": \"string\"\n\
  \    },\n    \"modificationPspReference\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The capture reference included in the transfer.\",\n      \"type\": \"string\"\n    },\n    \"panEntryMode\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"Indicates the method used for entering the PAN to initiate a transaction.\\n\\nPossible values: **manual**, **chip**, **magstripe**, **contactless**, **cof**, **ecommerce**, **token**.\",\n      \"enum\": [\n        \"chip\",\n        \"cof\",\n        \"contactless\",\n        \"ecommerce\",\n        \"magstripe\",\n        \"manual\",\n        \"token\"\n      ],\n      \"type\": \"string\"\n    },\n    \"paymentInstrument\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"Contains information about the payment instrument used in the transfer.\",\n      \"$ref\": \"#/components/schemas/PaymentInstrument\"\n    },\n    \"paymentInstrumentId\": {\n      \"description\": \"The unique identifier\
  \ of the source [payment instrument](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/paymentInstruments__resParam_id).\",\n      \"type\": \"string\"\n    },\n    \"paymentMerchantReference\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The payment's merchant reference included in the transfer.\",\n      \"type\": \"string\"\n    },\n    \"priority\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The priority for the bank transfer. This sets the speed at which the transfer is sent and the fees that you have to pay. Required for transfers with `category` **bank**.\\n\\nPossible values:\\n\\n* **regular**: For normal, low-value transactions.\\n\\n* **fast**: Faster way to transfer funds but has higher fees. Recommended for high-priority, low-value transactions.\\n\\n* **wire**: Fastest way to transfer funds but has the highest fees. Recommended for high-priority, high-value transactions.\\n\\n* **instant**: Instant way to transfer funds\
  \ in [SEPA countries](https://www.ecb.europa.eu/paym/integration/retail/sepa/html/index.en.html)\\n\\n.* **crossBorder**: High value transfer to receipt in a different country. \",\n      \"enum\": [\n        \"crossBorder\",\n        \"directDebit\",\n        \"fast\",\n        \"instant\",\n        \"regular\",\n        \"wire\"\n      ],\n      \"type\": \"string\"\n    },\n    \"processingType\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"Contains information about how the payment was processed. For example, **ecommerce** for online or **pos** for in-person payments.\",\n      \"enum\": [\n        \"atmWithdraw\",\n        \"balanceInquiry\",\n        \"ecommerce\",\n        \"moto\",\n        \"pos\",\n        \"purchaseWithCashback\",\n        \"recurring\",\n        \"token\"\n      ],\n      \"type\": \"string\"\n    },\n    \"pspPaymentReference\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The payment reference included in the transfer.\"\
  ,\n      \"type\": \"string\"\n    },\n    \"reason\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"Additional information about the status of the transfer.\",\n      \"enum\": [\n        \"amountLimitExceded\",\n        \"approved\",\n        \"counterpartyAccountBlocked\",\n        \"counterpartyAccountClosed\",\n        \"counterpartyAccountNotFound\",\n        \"counterpartyAddressRequired\",\n        \"counterpartyBankTimedOut\",\n        \"counterpartyBankUnavailable\",\n        \"error\",\n        \"notEnoughBalance\",\n        \"refusedByCounterpartyBank\",\n        \"routeNotFound\",\n        \"unknown\"\n      ],\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"Your reference for the transfer, used internally within your platform. If you don't provide this in the request, Adyen generates a unique reference.\",\n      \"maxLength\": 80,\n      \"type\": \"string\"\n    },\n    \"referenceForBeneficiary\"\
  : {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \" A reference that is sent to the recipient. This reference is also sent in all notification webhooks related to the transfer, so you can use it to track statuses for both the source and recipient of funds.\\n\\n Supported characters: **a-z**, **A-Z**, **0-9**. The maximum length depends on the `category`.\\n\\n- **internal**: 80 characters\\n\\n- **bank**: 35 characters when transferring to an IBAN, 15 characters for others.\",\n      \"maxLength\": 80,\n      \"type\": \"string\"\n    },\n    \"relayedAuthorisationData\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"If you are using relayed authorisation, this object contains information from the relayed authorisation response from your server.\",\n      \"$ref\": \"#/components/schemas/RelayedAuthorisationData-2\"\n    },\n    \"sequenceNumber\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The sequence number of the transfer notification.\
  \ The numbers start from 1 and increase with each new notification for a specific transfer.\\n\\nIt can help you restore the correct sequence of events even if they arrive out of order.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"status\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The result of the transfer.\\n\\n For example, **authorised**, **refused**, or **error**.\",\n      \"enum\": [\n        \"atmWithdrawal\",\n        \"atmWithdrawalReversalPending\",\n        \"atmWithdrawalReversed\",\n        \"authAdjustmentAuthorised\",\n        \"authAdjustmentError\",\n        \"authAdjustmentRefused\",\n        \"authorised\",\n        \"bankTransfer\",\n        \"bankTransferPending\",\n        \"booked\",\n        \"bookingPending\",\n        \"cancelled\",\n        \"capturePending\",\n        \"captureReversalPending\",\n        \"captureReversed\",\n        \"captured\",\n        \"chargeback\",\n        \"chargebackPending\"\
  ,\n        \"chargebackReversalPending\",\n        \"chargebackReversed\",\n        \"credited\",\n        \"depositCorrection\",\n        \"depositCorrectionPending\",\n        \"dispute\",\n        \"disputeClosed\",\n        \"disputeExpired\",\n        \"disputeNeedsReview\",\n        \"error\",\n        \"expired\",\n        \"failed\",\n        \"fee\",\n        \"feePending\",\n        \"internalTransfer\",\n        \"internalTransferPending\",\n        \"invoiceDeduction\",\n        \"invoiceDeductionPending\",\n        \"manualCorrectionPending\",\n        \"manuallyCorrected\",\n        \"matchedStatement\",\n        \"matchedStatementPending\",\n        \"merchantPayin\",\n        \"merchantPayinPending\",\n        \"merchantPayinReversed\",\n        \"merchantPayinReversedPending\",\n        \"miscCost\",\n        \"miscCostPending\",\n        \"paymentCost\",\n        \"paymentCostPending\",\n        \"received\",\n        \"refundPending\",\n        \"refundReversalPending\"\
  ,\n        \"refundReversed\",\n        \"refunded\",\n        \"refused\",\n        \"reserveAdjustment\",\n        \"reserveAdjustmentPending\",\n        \"returned\",\n        \"secondChargeback\",\n        \"secondChargebackPending\",\n        \"undefined\"\n      ],\n      \"type\": \"string\"\n    },\n    \"tracking\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The tracking information for the transfer.\",\n      \"$ref\": \"#/components/schemas/TransferNotificationTransferTracking\"\n    },\n    \"transactionId\": {\n      \"x-addedInVersion\": \"3\",\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"3\",\n      \"x-deprecatedMessage\": \"Use the [transactionId](https://docs.adyen.com/api-explorer/accounting-webhooks/latest/post/balancePlatform.transfer.created#request-data-events-transactionId) in the `events` array instead.\",\n      \"description\": \"The ID of the transaction that is created based on the transfer.\",\n      \"type\": \"string\"\
  \n    },\n    \"transactionRulesResult\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"Contains the results of the evaluation of the transaction rules.\",\n      \"$ref\": \"#/components/schemas/TransactionRulesResult\"\n    },\n    \"type\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The type of transfer or transaction. For example, **refund**, **payment**, **internalTransfer**, **bankTransfer**.\",\n      \"enum\": [\n        \"atmWithdrawal\",\n        \"atmWithdrawalReversal\",\n        \"balanceAdjustment\",\n        \"balanceRollover\",\n        \"bankTransfer\",\n        \"capture\",\n        \"captureReversal\",\n        \"chargeback\",\n        \"chargebackReversal\",\n        \"depositCorrection\",\n        \"fee\",\n        \"grant\",\n        \"installment\",\n        \"installmentReversal\",\n        \"internalTransfer\",\n        \"invoiceDeduction\",\n        \"leftover\",\n        \"manualCorrection\",\n        \"miscCost\",\n   \
  \     \"payment\",\n        \"paymentCost\",\n        \"refund\",\n        \"refundReversal\",\n        \"repayment\",\n        \"reserveAdjustment\",\n        \"secondChargeback\"\n      ],\n      \"type\": \"string\"\n    },\n    \"validationFacts\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The evaluation of the validation facts. See [validation checks](https://docs.adyen.com/issuing/validation-checks) for more information.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TransferNotificationValidationFact\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"category\",\n    \"amount\",\n    \"counterparty\",\n    \"status\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-transfer-notification-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransferNotificationData
---
