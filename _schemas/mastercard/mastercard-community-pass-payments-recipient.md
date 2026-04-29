---
description: Recipient Request
layout: schema
name: Recipient
properties_list:
- description: Client id generated for each beneficiary transaction by client application.
  name: clientId
  type: string
- description: Transcation id generated for each beneficiary transaction by payment provider.
  name: transactionId
  type: string
- description: Account Name
  name: accountName
  type: string
- description: Account Number
  name: accountNumber
  type: string
- description: Transaction Amount
  name: transactionAmount
  type: number
- description: Alphabetic code of currency as per ISO4217 standard.
  name: currency
  type: string
- description: ISO 3-alpha country code format.
  name: countryCode
  type: string
- description: Reason code
  name: responseCode
  type: string
- description: Response Message
  name: responseMessage
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-community-pass-payments-recipient-schema.json
slug: mastercard-community-pass-payments-recipient
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Recipient\",\n  \"type\": \"object\",\n  \"description\": \"Recipient Request\",\n  \"properties\": {\n    \"clientId\": {\n      \"type\": \"string\",\n      \"description\": \"Client id generated for each beneficiary transaction by client application.\"\n    },\n    \"transactionId\": {\n      \"type\": \"string\",\n      \"description\": \"Transcation id generated for each beneficiary transaction by payment provider.\"\n    },\n    \"accountName\": {\n      \"type\": \"string\",\n      \"description\": \"Account Name\"\n    },\n    \"accountNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Account Number\"\n    },\n    \"transactionAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Transaction Amount\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Alphabetic code of currency as per ISO4217 standard.\"\n    },\n    \"countryCode\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"ISO 3-alpha country code format.\"\n    },\n    \"responseCode\": {\n      \"type\": \"string\",\n      \"description\": \"Reason code\"\n    },\n    \"responseMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Response Message\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-community-pass-payments-recipient-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Recipient
---
