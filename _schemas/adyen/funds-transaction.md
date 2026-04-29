---
description: Transaction schema from Adyen API
layout: schema
name: Transaction
properties_list:
- description: The amount of the transaction.
  name: amount
  type: object
- description: The details of the bank account to where a payout was made.
  name: bankAccountDetail
  type: object
- description: The merchant reference of a related capture.
  name: captureMerchantReference
  type: string
- description: The psp reference of a related capture.
  name: capturePspReference
  type: string
- description: The date on which the transaction was performed.
  name: creationDate
  type: string
- description: A description of the transaction.
  name: description
  type: string
- description: The code of the account to which funds were credited during an outgoing fund transfer.
  name: destinationAccountCode
  type: string
- description: The psp reference of the related dispute.
  name: disputePspReference
  type: string
- description: The reason code of a dispute.
  name: disputeReasonCode
  type: string
- description: The merchant reference of a transaction.
  name: merchantReference
  type: string
- description: The psp reference of the related authorisation or transfer.
  name: paymentPspReference
  type: string
- description: The psp reference of the related payout.
  name: payoutPspReference
  type: string
- description: The psp reference of a transaction.
  name: pspReference
  type: string
- description: The code of the account from which funds were debited during an incoming fund transfer.
  name: sourceAccountCode
  type: string
- description: 'The status of the transaction. >Permitted values: `PendingCredit`, `CreditFailed`, `CreditClosed`, `CreditSuspended`, `Credited`, `Converted`, `PendingDebit`, `DebitFailed`, `Debited`, `DebitReversedR'
  name: transactionStatus
  type: string
- description: The transfer code of the transaction.
  name: transferCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/funds-transaction-schema.json
slug: funds-transaction
source_filename: funds-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-transaction-schema.json\",\n  \"title\": \"Transaction\",\n  \"description\": \"Transaction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"The amount of the transaction.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"bankAccountDetail\": {\n      \"description\": \"The details of the bank account to where a payout was made.\",\n      \"$ref\": \"#/components/schemas/BankAccountDetail\"\n    },\n    \"captureMerchantReference\": {\n      \"description\": \"The merchant reference of a related capture.\",\n      \"type\": \"string\"\n    },\n    \"capturePspReference\": {\n      \"description\": \"The psp reference of a related capture.\",\n      \"type\": \"string\"\n    },\n    \"creationDate\": {\n      \"description\"\
  : \"The date on which the transaction was performed.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"A description of the transaction.\",\n      \"type\": \"string\"\n    },\n    \"destinationAccountCode\": {\n      \"description\": \"The code of the account to which funds were credited during an outgoing fund transfer.\",\n      \"type\": \"string\"\n    },\n    \"disputePspReference\": {\n      \"description\": \"The psp reference of the related dispute.\",\n      \"type\": \"string\"\n    },\n    \"disputeReasonCode\": {\n      \"description\": \"The reason code of a dispute.\",\n      \"type\": \"string\"\n    },\n    \"merchantReference\": {\n      \"description\": \"The merchant reference of a transaction.\",\n      \"type\": \"string\"\n    },\n    \"paymentPspReference\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The psp reference of the related authorisation or transfer.\",\n     \
  \ \"type\": \"string\"\n    },\n    \"payoutPspReference\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The psp reference of the related payout.\",\n      \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"description\": \"The psp reference of a transaction.\",\n      \"type\": \"string\"\n    },\n    \"sourceAccountCode\": {\n      \"description\": \"The code of the account from which funds were debited during an incoming fund transfer.\",\n      \"type\": \"string\"\n    },\n    \"transactionStatus\": {\n      \"description\": \"The status of the transaction.\\n>Permitted values: `PendingCredit`, `CreditFailed`, `CreditClosed`, `CreditSuspended`, `Credited`, `Converted`, `PendingDebit`, `DebitFailed`, `Debited`, `DebitReversedReceived`, `DebitedReversed`, `ChargebackReceived`, `Chargeback`, `ChargebackReversedReceived`, `ChargebackReversed`, `Payout`, `PayoutReversed`, `FundTransfer`, `PendingFundTransfer`, `ManualCorrected`.\",\n      \"enum\": [\n  \
  \      \"BalanceNotPaidOutTransfer\",\n        \"BalancePlatformSweep\",\n        \"BalancePlatformSweepReturned\",\n        \"Chargeback\",\n        \"ChargebackCorrection\",\n        \"ChargebackCorrectionReceived\",\n        \"ChargebackReceived\",\n        \"ChargebackReversed\",\n        \"ChargebackReversedCorrection\",\n        \"ChargebackReversedCorrectionReceived\",\n        \"ChargebackReversedReceived\",\n        \"Converted\",\n        \"CreditClosed\",\n        \"CreditFailed\",\n        \"CreditReversed\",\n        \"CreditReversedReceived\",\n        \"CreditSuspended\",\n        \"Credited\",\n        \"DebitFailed\",\n        \"DebitReversedReceived\",\n        \"Debited\",\n        \"DebitedReversed\",\n        \"DepositCorrectionCredited\",\n        \"DepositCorrectionDebited\",\n        \"Fee\",\n        \"FundTransfer\",\n        \"FundTransferReversed\",\n        \"InvoiceDeductionCredited\",\n        \"InvoiceDeductionDebited\",\n        \"ManualCorrected\",\n \
  \       \"ManualCorrectionCredited\",\n        \"ManualCorrectionDebited\",\n        \"MerchantPayin\",\n        \"MerchantPayinReversed\",\n        \"Payout\",\n        \"PayoutReversed\",\n        \"PendingCredit\",\n        \"PendingDebit\",\n        \"PendingFundTransfer\",\n        \"ReCredited\",\n        \"ReCreditedReceived\",\n        \"SecondChargeback\",\n        \"SecondChargebackCorrection\",\n        \"SecondChargebackCorrectionReceived\",\n        \"SecondChargebackReceived\"\n      ],\n      \"type\": \"string\"\n    },\n    \"transferCode\": {\n      \"description\": \"The transfer code of the transaction.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-transaction-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Transaction
---
