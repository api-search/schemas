---
description: A Barclays account transaction as returned by the Transactions API.
layout: schema
name: Transaction
properties_list:
- description: Account identifier the transaction belongs to.
  name: accountId
  type: string
- description: Unique transaction identifier.
  name: transactionId
  type: string
- description: Whether the transaction credits or debits the account.
  name: creditDebitIndicator
  type: string
- description: Settlement status of the transaction.
  name: status
  type: string
- description: Date and time the transaction was booked.
  name: bookingDateTime
  type: string
- description: Value date and time of the transaction.
  name: valueDateTime
  type: string
- description: ''
  name: amount
  type: object
- description: ''
  name: merchantDetails
  type: object
- description: Narrative description of the transaction.
  name: transactionInformation
  type: string
provider_name: Barclays
provider_slug: barclays
schema_file: json-schema/transaction-schema.json
slug: transaction
tags:
- Banking
- Credit Cards
- Finance
- Open Banking
- Payments
- PSD2
- UK Banking
title: Transaction
---
