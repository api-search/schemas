---
description: A payment transaction processed through Montran's payment infrastructure. Aligned with ISO 20022 payment messaging standards including pain.001 (CustomerCreditTransferInitiation), pacs.008 (FIToFICustomerCreditTransfer), and pacs.002 (FIToFIPaymentStatusReport).
layout: schema
name: Montran Payment
properties_list:
- description: Unique payment identifier assigned by the system
  name: paymentId
  type: string
- description: Unique message identification assigned by the initiating party (ISO 20022 MsgId)
  name: messageId
  type: string
- description: End-to-end identification assigned by the initiating party, passed through the entire payment chain (ISO 20022 EndToEndId)
  name: endToEndId
  type: string
- description: Unique transaction identification assigned by the first instructing agent (ISO 20022 TxId)
  name: transactionId
  type: string
- description: Type of payment transaction
  name: paymentType
  type: string
- description: Current payment processing status using ISO 20022 status codes
  name: status
  type: string
- description: Reason code for rejection or return (ISO 20022 reason codes)
  name: statusReasonCode
  type: string
- description: Human-readable description of the status reason
  name: statusReasonDescription
  type: string
- description: Name of the debtor (payer/originator)
  name: debtorName
  type: string
- description: ''
  name: debtorAccount
  type: object
- description: ''
  name: debtorAgent
  type: object
- description: Name of the creditor (payee/beneficiary)
  name: creditorName
  type: string
- description: ''
  name: creditorAccount
  type: object
- description: ''
  name: creditorAgent
  type: object
- description: Payment amount
  name: amount
  type: number
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Requested execution date for the payment
  name: requestedExecutionDate
  type: string
- description: Actual or expected settlement date
  name: settlementDate
  type: string
- description: Clearing and settlement mechanism used
  name: clearingSystem
  type: string
- description: Remittance information or payment reference
  name: remittanceInformation
  type: string
- description: Specifies which party bears the charges
  name: chargeBearer
  type: string
- description: Service level code (e.g., SEPA, URGP)
  name: serviceLevel
  type: string
- description: Category purpose code for the payment
  name: categoryPurpose
  type: string
- description: Timestamp when the payment was created
  name: createdAt
  type: string
- description: Timestamp of the last status update
  name: updatedAt
  type: string
provider_name: Montran
provider_slug: montran
schema_file: json-schema/montran-payment-schema.json
slug: montran-payment
source_filename: montran-payment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.montran.com/schemas/payment.json\",\n  \"title\": \"Montran Payment\",\n  \"description\": \"A payment transaction processed through Montran's payment infrastructure. Aligned with ISO 20022 payment messaging standards including pain.001 (CustomerCreditTransferInitiation), pacs.008 (FIToFICustomerCreditTransfer), and pacs.002 (FIToFIPaymentStatusReport).\",\n  \"type\": \"object\",\n  \"required\": [\n    \"paymentId\",\n    \"paymentType\",\n    \"debtorAccount\",\n    \"creditorAccount\",\n    \"amount\",\n    \"currency\",\n    \"status\"\n  ],\n  \"properties\": {\n    \"paymentId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique payment identifier assigned by the system\"\n    },\n    \"messageId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique message identification assigned by the initiating party (ISO 20022 MsgId)\"\n    },\n    \"endToEndId\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"End-to-end identification assigned by the initiating party, passed through the entire payment chain (ISO 20022 EndToEndId)\"\n    },\n    \"transactionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique transaction identification assigned by the first instructing agent (ISO 20022 TxId)\"\n    },\n    \"paymentType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of payment transaction\",\n      \"enum\": [\n        \"credit-transfer\",\n        \"direct-debit\",\n        \"instant-payment\",\n        \"cross-border\",\n        \"cheque\",\n        \"remittance\",\n        \"request-to-pay\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current payment processing status using ISO 20022 status codes\",\n      \"enum\": [\n        \"RCVD\",\n        \"ACTC\",\n        \"ACCP\",\n        \"ACSP\",\n        \"ACSC\",\n        \"ACWC\",\n        \"PDNG\",\n\
  \        \"RJCT\",\n        \"CANC\",\n        \"RTND\"\n      ]\n    },\n    \"statusReasonCode\": {\n      \"type\": \"string\",\n      \"description\": \"Reason code for rejection or return (ISO 20022 reason codes)\"\n    },\n    \"statusReasonDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the status reason\"\n    },\n    \"debtorName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the debtor (payer/originator)\"\n    },\n    \"debtorAccount\": {\n      \"$ref\": \"#/$defs/AccountIdentification\"\n    },\n    \"debtorAgent\": {\n      \"$ref\": \"#/$defs/FinancialInstitution\"\n    },\n    \"creditorName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the creditor (payee/beneficiary)\"\n    },\n    \"creditorAccount\": {\n      \"$ref\": \"#/$defs/AccountIdentification\"\n    },\n    \"creditorAgent\": {\n      \"$ref\": \"#/$defs/FinancialInstitution\"\n    },\n    \"amount\": {\n      \"\
  type\": \"number\",\n      \"description\": \"Payment amount\",\n      \"minimum\": 0.01\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"requestedExecutionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Requested execution date for the payment\"\n    },\n    \"settlementDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Actual or expected settlement date\"\n    },\n    \"clearingSystem\": {\n      \"type\": \"string\",\n      \"description\": \"Clearing and settlement mechanism used\",\n      \"enum\": [\n        \"SEPA\",\n        \"TARGET2\",\n        \"FEDWIRE\",\n        \"CHIPS\",\n        \"CHAPS\",\n        \"FASTER_PAYMENTS\",\n        \"TIPS\",\n        \"RT1\",\n        \"RTGS\",\n        \"ACH\",\n        \"SWIFT\"\n      ]\n    },\n    \"remittanceInformation\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Remittance information or payment reference\"\n    },\n    \"chargeBearer\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies which party bears the charges\",\n      \"enum\": [\n        \"DEBT\",\n        \"CRED\",\n        \"SHAR\",\n        \"SLEV\"\n      ]\n    },\n    \"serviceLevel\": {\n      \"type\": \"string\",\n      \"description\": \"Service level code (e.g., SEPA, URGP)\"\n    },\n    \"categoryPurpose\": {\n      \"type\": \"string\",\n      \"description\": \"Category purpose code for the payment\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the payment was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last status update\"\n    }\n  },\n  \"$defs\": {\n    \"AccountIdentification\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Account identification using IBAN or proprietary account number\",\n      \"properties\": {\n        \"iban\": {\n          \"type\": \"string\",\n          \"description\": \"International Bank Account Number\",\n          \"pattern\": \"^[A-Z]{2}[0-9]{2}[A-Z0-9]{4,30}$\"\n        },\n        \"accountNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Proprietary account number\"\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"description\": \"Account currency (ISO 4217)\",\n          \"pattern\": \"^[A-Z]{3}$\"\n        }\n      }\n    },\n    \"FinancialInstitution\": {\n      \"type\": \"object\",\n      \"description\": \"Financial institution identification\",\n      \"properties\": {\n        \"bic\": {\n          \"type\": \"string\",\n          \"description\": \"Bank Identifier Code (SWIFT/BIC)\",\n          \"pattern\": \"^[A-Z]{4}[A-Z]{2}[A-Z0-9]{2}([A-Z0-9]{3})?$\"\n        },\n        \"name\": {\n          \"\
  type\": \"string\",\n          \"description\": \"Name of the financial institution\"\n        },\n        \"clearingSystemMemberId\": {\n          \"type\": \"string\",\n          \"description\": \"Clearing system member identification\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/montran/refs/heads/main/json-schema/montran-payment-schema.json
tags:
- Banking
- Central Banking
- Financial Services
- ISO 20022
- Market Infrastructure
- Messaging
- Payments
- Real-Time Payments
- SWIFT
title: Montran Payment
---
