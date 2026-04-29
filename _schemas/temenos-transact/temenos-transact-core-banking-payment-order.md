---
description: A payment order in Temenos Transact for submitting payment instructions through various clearing systems.
layout: schema
name: PaymentOrder
properties_list:
- description: Unique payment order identifier
  name: paymentOrderId
  type: string
- description: Debit account identifier
  name: debitAccountId
  type: string
- description: Amount debited from the source account
  name: debitAmount
  type: number
- description: Currency of the debit
  name: debitCurrency
  type: string
- description: Credit account identifier or beneficiary account
  name: creditAccountId
  type: string
- description: Amount credited to the destination account
  name: creditAmount
  type: number
- description: Currency of the credit
  name: creditCurrency
  type: string
- description: Payment type classification
  name: paymentType
  type: string
- description: Payment order status
  name: status
  type: string
- description: Value date of the payment
  name: valueDate
  type: string
- description: Timestamp when the payment was executed
  name: executionDate
  type: string
- description: Name of the payment beneficiary
  name: beneficiaryName
  type: string
- description: IBAN of the beneficiary
  name: beneficiaryIban
  type: string
- description: BIC/SWIFT code of the beneficiary bank
  name: beneficiaryBic
  type: string
- description: Remittance information or payment reference
  name: remittanceInformation
  type: string
- description: Who bears the charges
  name: chargesType
  type: string
- description: Total charges applied
  name: totalCharges
  type: number
- description: Applied exchange rate
  name: exchangeRate
  type: number
- description: Reason for rejection if applicable
  name: rejectionReason
  type: string
provider_name: Temenos Transact
provider_slug: temenos-transact
schema_file: json-schema/temenos-transact-core-banking-payment-order-schema.json
slug: temenos-transact-core-banking-payment-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaymentOrder\",\n  \"type\": \"object\",\n  \"description\": \"A payment order in Temenos Transact for submitting payment instructions through various clearing systems.\",\n  \"properties\": {\n    \"paymentOrderId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique payment order identifier\"\n    },\n    \"debitAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"Debit account identifier\"\n    },\n    \"debitAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Amount debited from the source account\"\n    },\n    \"debitCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency of the debit\"\n    },\n    \"creditAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"Credit account identifier or beneficiary account\"\n    },\n    \"creditAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Amount\
  \ credited to the destination account\"\n    },\n    \"creditCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency of the credit\"\n    },\n    \"paymentType\": {\n      \"type\": \"string\",\n      \"description\": \"Payment type classification\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Payment order status\"\n    },\n    \"valueDate\": {\n      \"type\": \"string\",\n      \"description\": \"Value date of the payment\"\n    },\n    \"executionDate\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the payment was executed\"\n    },\n    \"beneficiaryName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the payment beneficiary\"\n    },\n    \"beneficiaryIban\": {\n      \"type\": \"string\",\n      \"description\": \"IBAN of the beneficiary\"\n    },\n    \"beneficiaryBic\": {\n      \"type\": \"string\",\n      \"description\": \"BIC/SWIFT code of the beneficiary bank\"\n    },\n\
  \    \"remittanceInformation\": {\n      \"type\": \"string\",\n      \"description\": \"Remittance information or payment reference\"\n    },\n    \"chargesType\": {\n      \"type\": \"string\",\n      \"description\": \"Who bears the charges\"\n    },\n    \"totalCharges\": {\n      \"type\": \"number\",\n      \"description\": \"Total charges applied\"\n    },\n    \"exchangeRate\": {\n      \"type\": \"number\",\n      \"description\": \"Applied exchange rate\"\n    },\n    \"rejectionReason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for rejection if applicable\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/json-schema/temenos-transact-core-banking-payment-order-schema.json
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
title: PaymentOrder
---
