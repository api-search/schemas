---
description: notification request
layout: schema
name: Notification
properties_list:
- description: Application identifier for client.
  name: appId
  type: string
- description: 'Code to identify partner. Eg: school on Kupaa'
  name: partnerId
  type: string
- description: Unique transaction ID from Payment Provider
  name: providerReference
  type: string
- description: Payer mobile bank account number
  name: srcAccount
  type: string
- description: Depicts mode of payment as mentioned in enum.
  name: paymentChannel
  type: string
- description: Transaction amount
  name: transactionAmount
  type: number
- description: Payer's account id
  name: accountId
  type: string
- description: Transaction date in the format 'YYYY-MM-DD'
  name: transactionDate
  type: string
- description: Description of payment
  name: narration
  type: string
- description: Payer Name
  name: accountName
  type: string
- description: Destination account number
  name: accountNumber
  type: string
- description: Alphabetic code of currency as per ISO4217 standard.
  name: currency
  type: string
- description: ISO 3-alpha country code format.
  name: countryCode
  type: string
- description: Signature for request
  name: signature
  type: string
- description: CorrelationId for request
  name: correlationId
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-community-pass-payments-notification-schema.json
slug: mastercard-community-pass-payments-notification
source_filename: mastercard-community-pass-payments-notification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Notification\",\n  \"type\": \"object\",\n  \"description\": \"notification request\",\n  \"properties\": {\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\": \"Application identifier for client.\"\n    },\n    \"partnerId\": {\n      \"type\": \"string\",\n      \"description\": \"Code to identify partner. Eg: school on Kupaa\"\n    },\n    \"providerReference\": {\n      \"type\": \"string\",\n      \"description\": \"Unique transaction ID from Payment Provider\"\n    },\n    \"srcAccount\": {\n      \"type\": \"string\",\n      \"description\": \"Payer mobile bank account number\"\n    },\n    \"paymentChannel\": {\n      \"type\": \"string\",\n      \"description\": \"Depicts mode of payment as mentioned in enum.\"\n    },\n    \"transactionAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Transaction amount\"\n    },\n    \"accountId\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Payer's account id\"\n    },\n    \"transactionDate\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction date in the format 'YYYY-MM-DD'\"\n    },\n    \"narration\": {\n      \"type\": \"string\",\n      \"description\": \"Description of payment\"\n    },\n    \"accountName\": {\n      \"type\": \"string\",\n      \"description\": \"Payer Name\"\n    },\n    \"accountNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Destination account number\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Alphabetic code of currency as per ISO4217 standard.\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3-alpha country code format.\"\n    },\n    \"signature\": {\n      \"type\": \"string\",\n      \"description\": \"Signature for request\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"description\": \"CorrelationId for\
  \ request\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-community-pass-payments-notification-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Notification
---
