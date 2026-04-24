---
description: An account statement
layout: schema
name: Statement
properties_list:
- description: Unique statement identifier
  name: statementId
  type: string
- description: Associated account ID
  name: accountId
  type: string
- description: Statement date
  name: statementDate
  type: string
- description: ''
  name: openingBalance
  type: number
- description: ''
  name: closingBalance
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: totalCredits
  type: number
- description: ''
  name: totalDebits
  type: number
- description: ''
  name: transactionCount
  type: integer
provider_name: Bank of America
provider_slug: bank-of-america
schema_file: json-schema/statement-schema.json
slug: statement
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
title: Statement
---
