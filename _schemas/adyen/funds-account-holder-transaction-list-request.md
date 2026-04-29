---
description: AccountHolderTransactionListRequest schema from Adyen API
layout: schema
name: AccountHolderTransactionListRequest
properties_list:
- description: The code of the account holder that owns the account(s) of which retrieve the transaction list.
  name: accountHolderCode
  type: string
- description: A list of accounts to include in the transaction list. If left blank, the last fifty (50) transactions for all accounts of the account holder will be included.
  name: transactionListsPerAccount
  type: array
- description: 'A list of statuses to include in the transaction list. If left blank, all transactions will be included. >Permitted values: >* `PendingCredit` - a pending balance credit. >* `CreditFailed` - a pending'
  name: transactionStatuses
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/funds-account-holder-transaction-list-request-schema.json
slug: funds-account-holder-transaction-list-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-account-holder-transaction-list-request-schema.json\",\n  \"title\": \"AccountHolderTransactionListRequest\",\n  \"description\": \"AccountHolderTransactionListRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"The code of the account holder that owns the account(s) of which retrieve the transaction list.\",\n      \"type\": \"string\"\n    },\n    \"transactionListsPerAccount\": {\n      \"description\": \"A list of accounts to include in the transaction list. If left blank, the last fifty (50) transactions for all accounts of the account holder will be included.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TransactionListForAccount\"\n      },\n      \"type\": \"array\"\n    },\n    \"transactionStatuses\"\
  : {\n      \"description\": \"A list of statuses to include in the transaction list. If left blank, all transactions will be included.\\n>Permitted values:\\n>* `PendingCredit` - a pending balance credit.\\n>* `CreditFailed` - a pending credit failure; the balance will not be credited.\\n>* `Credited` - a credited balance.\\n>* `PendingDebit` - a pending balance debit (e.g., a refund).\\n>* `CreditClosed` - a pending credit closed; the balance will not be credited.\\n>* `CreditSuspended` - a pending credit closed; the balance will not be credited.\\n>* `DebitFailed` - a pending debit failure; the balance will not be debited.\\n>* `Debited` - a debited balance (e.g., a refund).\\n>* `DebitReversedReceived` - a pending refund reversal.\\n>* `DebitedReversed` - a reversed refund.\\n>* `ChargebackReceived` - a received chargeback request.\\n>* `Chargeback` - a processed chargeback.\\n>* `ChargebackReversedReceived` - a pending chargeback reversal.\\n>* `ChargebackReversed` - a reversed chargeback.\\\
  n>* `Converted` - converted.\\n>* `ManualCorrected` - manual booking/adjustment by Adyen.\\n>* `Payout` - a payout.\\n>* `PayoutReversed` - a reversed payout.\\n>* `PendingFundTransfer` - a pending transfer of funds from one account to another.\\n>* `FundTransfer` - a transfer of funds from one account to another.\",\n      \"items\": {\n        \"enum\": [\n          \"BalanceNotPaidOutTransfer\",\n          \"BalancePlatformSweep\",\n          \"BalancePlatformSweepReturned\",\n          \"Chargeback\",\n          \"ChargebackCorrection\",\n          \"ChargebackCorrectionReceived\",\n          \"ChargebackReceived\",\n          \"ChargebackReversed\",\n          \"ChargebackReversedCorrection\",\n          \"ChargebackReversedCorrectionReceived\",\n          \"ChargebackReversedReceived\",\n          \"Converted\",\n          \"CreditClosed\",\n          \"CreditFailed\",\n          \"CreditReversed\",\n          \"CreditReversedReceived\",\n          \"CreditSuspended\",\n        \
  \  \"Credited\",\n          \"DebitFailed\",\n          \"DebitReversedReceived\",\n          \"Debited\",\n          \"DebitedReversed\",\n          \"DepositCorrectionCredited\",\n          \"DepositCorrectionDebited\",\n          \"Fee\",\n          \"FundTransfer\",\n          \"FundTransferReversed\",\n          \"InvoiceDeductionCredited\",\n          \"InvoiceDeductionDebited\",\n          \"ManualCorrected\",\n          \"ManualCorrectionCredited\",\n          \"ManualCorrectionDebited\",\n          \"MerchantPayin\",\n          \"MerchantPayinReversed\",\n          \"Payout\",\n          \"PayoutReversed\",\n          \"PendingCredit\",\n          \"PendingDebit\",\n          \"PendingFundTransfer\",\n          \"ReCredited\",\n          \"ReCreditedReceived\",\n          \"SecondChargeback\",\n          \"SecondChargebackCorrection\",\n          \"SecondChargebackCorrectionReceived\",\n          \"SecondChargebackReceived\"\n        ],\n        \"type\": \"string\"\n      },\n\
  \      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"accountHolderCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-account-holder-transaction-list-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountHolderTransactionListRequest
---
