---
description: A loan arrangement in Temenos Transact
layout: schema
name: Loan
properties_list:
- description: Unique loan identifier
  name: loanId
  type: string
- description: Customer identifier
  name: customerId
  type: string
- description: Loan product identifier
  name: productId
  type: string
- description: Name of the loan product
  name: productName
  type: string
- description: Original loan principal amount
  name: principalAmount
  type: number
- description: Current outstanding balance
  name: outstandingBalance
  type: number
- description: Loan currency
  name: currency
  type: string
- description: Applied interest rate percentage
  name: interestRate
  type: number
- description: Annual percentage rate (APR)
  name: effectiveRate
  type: number
- description: Date the loan was disbursed
  name: disbursementDate
  type: string
- description: Loan maturity date
  name: maturityDate
  type: string
- description: Next repayment due date
  name: nextPaymentDate
  type: string
- description: Next repayment amount due
  name: nextPaymentAmount
  type: number
- description: Frequency of loan repayments
  name: repaymentFrequency
  type: string
- description: Loan status
  name: status
  type: string
- description: Amount currently overdue
  name: overdueAmount
  type: number
- description: Number of days past due
  name: daysPastDue
  type: integer
provider_name: Temenos Transact
provider_slug: temenos-transact
schema_file: json-schema/temenos-transact-core-banking-loan-schema.json
slug: temenos-transact-core-banking-loan
source_filename: temenos-transact-core-banking-loan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Loan\",\n  \"type\": \"object\",\n  \"description\": \"A loan arrangement in Temenos Transact\",\n  \"properties\": {\n    \"loanId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique loan identifier\"\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Customer identifier\"\n    },\n    \"productId\": {\n      \"type\": \"string\",\n      \"description\": \"Loan product identifier\"\n    },\n    \"productName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the loan product\"\n    },\n    \"principalAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Original loan principal amount\"\n    },\n    \"outstandingBalance\": {\n      \"type\": \"number\",\n      \"description\": \"Current outstanding balance\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Loan currency\"\n    },\n\
  \    \"interestRate\": {\n      \"type\": \"number\",\n      \"description\": \"Applied interest rate percentage\"\n    },\n    \"effectiveRate\": {\n      \"type\": \"number\",\n      \"description\": \"Annual percentage rate (APR)\"\n    },\n    \"disbursementDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date the loan was disbursed\"\n    },\n    \"maturityDate\": {\n      \"type\": \"string\",\n      \"description\": \"Loan maturity date\"\n    },\n    \"nextPaymentDate\": {\n      \"type\": \"string\",\n      \"description\": \"Next repayment due date\"\n    },\n    \"nextPaymentAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Next repayment amount due\"\n    },\n    \"repaymentFrequency\": {\n      \"type\": \"string\",\n      \"description\": \"Frequency of loan repayments\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Loan status\"\n    },\n    \"overdueAmount\": {\n      \"type\": \"number\",\n      \"description\"\
  : \"Amount currently overdue\"\n    },\n    \"daysPastDue\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of days past due\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/json-schema/temenos-transact-core-banking-loan-schema.json
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
title: Loan
---
