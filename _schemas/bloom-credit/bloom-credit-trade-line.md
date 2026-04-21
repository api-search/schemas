---
description: An individual account or trade line in a credit report.
layout: schema
name: TradeLine
properties_list:
- description: Unique identifier for this trade line.
  name: account_id
  type: string
- description: Bureau reporting this trade line.
  name: bureau
  type: string
- description: Name of the creditor or lender.
  name: creditor_name
  type: string
- description: Type of account.
  name: account_type
  type: string
- description: Whether the account is open or closed.
  name: account_status
  type: string
- description: Credit limit in USD.
  name: credit_limit
  type: integer
- description: Current balance in USD.
  name: current_balance
  type: integer
- description: Current payment status.
  name: payment_status
  type: string
- description: ''
  name: opened_date
  type: string
- description: ''
  name: last_activity_date
  type: string
provider_name: Bloom Credit
provider_slug: bloom-credit
schema_file: json-schema/bloom-credit-trade-line-schema.json
slug: bloom-credit-trade-line
tags:
- Credit Bureau
- Credit Reports
- Credit Scores
- Fintech
- Lending
- Personal Finance
title: TradeLine
---
