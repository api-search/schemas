---
description: Schema for Temenos payment orders including domestic transfers, international SWIFT payments, SEPA credit transfers, and internal account transfers with full ISO 20022 support.
layout: schema
name: Temenos Payment Order
properties_list:
- description: Unique payment order identifier assigned by the system
  name: paymentOrderId
  type: string
- description: Identifier of the originating debit account
  name: debitAccountId
  type: string
- description: Identifier of the destination credit account for internal transfers
  name: creditAccountId
  type: string
- description: Payment amount in the specified currency
  name: amount
  type: number
- description: Payment currency in ISO 4217 format
  name: currency
  type: string
- description: Classification of the payment type determining the clearing channel
  name: paymentType
  type: string
- description: Current processing status of the payment order
  name: status
  type: string
- description: Requested value date for the payment
  name: valueDate
  type: string
- description: Actual execution date when the payment was processed
  name: executionDate
  type:
  - string
  - 'null'
- description: Payment reference provided by the originator
  name: reference
  type: string
- description: End-to-end identifier for ISO 20022 payment tracking
  name: endToEndId
  type: string
- description: ''
  name: beneficiary
  type: object
- description: Remittance information accompanying the payment
  name: remittanceInformation
  type: string
- description: Charge allocation between originator and beneficiary
  name: chargeBearer
  type: string
- description: Status within the clearing system
  name: clearingStatus
  type: string
- description: Account booking status
  name: bookingStatus
  type: string
- description: Reason for payment failure if applicable
  name: failureReason
  type:
  - string
  - 'null'
- description: Timestamp when the payment order was created
  name: createdDate
  type: string
- description: Timestamp of the last status update
  name: lastUpdated
  type: string
provider_name: Temenos
provider_slug: temenos
schema_file: json-schema/temenos-payment-order-schema.json
slug: temenos-payment-order
source_filename: temenos-payment-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://temenos.com/schemas/temenos/payment-order.json\",\n  \"title\": \"Temenos Payment Order\",\n  \"description\": \"Schema for Temenos payment orders including domestic transfers, international SWIFT payments, SEPA credit transfers, and internal account transfers with full ISO 20022 support.\",\n  \"type\": \"object\",\n  \"required\": [\"paymentOrderId\", \"debitAccountId\", \"amount\", \"currency\", \"paymentType\", \"status\"],\n  \"properties\": {\n    \"paymentOrderId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique payment order identifier assigned by the system\"\n    },\n    \"debitAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the originating debit account\"\n    },\n    \"creditAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the destination credit account for internal transfers\"\n    },\n\
  \    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Payment amount in the specified currency\",\n      \"minimum\": 0.01\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Payment currency in ISO 4217 format\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"paymentType\": {\n      \"type\": \"string\",\n      \"description\": \"Classification of the payment type determining the clearing channel\",\n      \"enum\": [\n        \"INTERNAL\",\n        \"DOMESTIC\",\n        \"INTERNATIONAL\",\n        \"SEPA_CREDIT\",\n        \"INSTANT_SEPA\",\n        \"SWIFT\",\n        \"TARGET2\",\n        \"CROSS_BORDER\",\n        \"ACH\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current processing status of the payment order\",\n      \"enum\": [\"PENDING\", \"PROCESSING\", \"COMPLETED\", \"FAILED\", \"CANCELLED\", \"RETURNED\"]\n    },\n    \"valueDate\": {\n      \"type\": \"string\",\n    \
  \  \"format\": \"date\",\n      \"description\": \"Requested value date for the payment\"\n    },\n    \"executionDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Actual execution date when the payment was processed\"\n    },\n    \"reference\": {\n      \"type\": \"string\",\n      \"description\": \"Payment reference provided by the originator\",\n      \"maxLength\": 140\n    },\n    \"endToEndId\": {\n      \"type\": \"string\",\n      \"description\": \"End-to-end identifier for ISO 20022 payment tracking\",\n      \"maxLength\": 35\n    },\n    \"beneficiary\": {\n      \"$ref\": \"#/$defs/Beneficiary\"\n    },\n    \"remittanceInformation\": {\n      \"type\": \"string\",\n      \"description\": \"Remittance information accompanying the payment\",\n      \"maxLength\": 140\n    },\n    \"chargeBearer\": {\n      \"type\": \"string\",\n      \"description\": \"Charge allocation between originator and beneficiary\",\n      \"\
  enum\": [\"SHA\", \"OUR\", \"BEN\"]\n    },\n    \"clearingStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Status within the clearing system\"\n    },\n    \"bookingStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Account booking status\",\n      \"enum\": [\"BOOKED\", \"PENDING\", \"REJECTED\"]\n    },\n    \"failureReason\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Reason for payment failure if applicable\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the payment order was created\"\n    },\n    \"lastUpdated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last status update\"\n    }\n  },\n  \"$defs\": {\n    \"Beneficiary\": {\n      \"type\": \"object\",\n      \"description\": \"Payment beneficiary details\",\n      \"properties\": {\n        \"name\": {\n        \
  \  \"type\": \"string\",\n          \"description\": \"Beneficiary name\",\n          \"maxLength\": 140\n        },\n        \"iban\": {\n          \"type\": \"string\",\n          \"description\": \"Beneficiary International Bank Account Number\",\n          \"pattern\": \"^[A-Z]{2}[0-9]{2}[A-Z0-9]{4,30}$\"\n        },\n        \"bic\": {\n          \"type\": \"string\",\n          \"description\": \"Beneficiary bank BIC/SWIFT code\",\n          \"pattern\": \"^[A-Z]{4}[A-Z]{2}[A-Z0-9]{2}([A-Z0-9]{3})?$\"\n        },\n        \"accountNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Beneficiary account number for non-IBAN payments\"\n        },\n        \"bankName\": {\n          \"type\": \"string\",\n          \"description\": \"Beneficiary bank name\"\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"Beneficiary address\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Beneficiary country in ISO 3166-1 alpha-2 format\",\n          \"pattern\": \"^[A-Z]{2}$\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/json-schema/temenos-payment-order-schema.json
tags:
- Banking
- Cloud Banking
- Core Banking
- Digital Banking
- Financial Services
- Fintech
- Open Banking
- Payments
- Wealth Management
title: Temenos Payment Order
---
