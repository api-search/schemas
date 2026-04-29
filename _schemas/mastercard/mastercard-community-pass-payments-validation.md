---
description: Validation Request
layout: schema
name: Validation
properties_list:
- description: Application identifier for client.
  name: appId
  type: string
- description: 'Code to identify partner. E,g: school on Kupaa.'
  name: partnerId
  type: string
- description: 'Account Number being validated. E.g: student id.'
  name: accountId
  type: string
- description: Partner type can be one of values in enum.
  name: partnerType
  type: string
- description: Correlation Id for tracking request
  name: correlationId
  type: string
- description: Transaction time in the format 'YYYY-MM-DDThh:mm:ssTZD'
  name: transactionTime
  type: string
- description: Depicts mode of payment as mentioned in enum.
  name: paymentChannel
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-community-pass-payments-validation-schema.json
slug: mastercard-community-pass-payments-validation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Validation\",\n  \"type\": \"object\",\n  \"description\": \"Validation Request\",\n  \"properties\": {\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\": \"Application identifier for client.\"\n    },\n    \"partnerId\": {\n      \"type\": \"string\",\n      \"description\": \"Code to identify partner. E,g: school on Kupaa.\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Account Number being validated. E.g: student id.\"\n    },\n    \"partnerType\": {\n      \"type\": \"string\",\n      \"description\": \"Partner type can be one of values in enum.\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"description\": \"Correlation Id for tracking request\"\n    },\n    \"transactionTime\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction time in the format 'YYYY-MM-DDThh:mm:ssTZD'\"\n    },\n \
  \   \"paymentChannel\": {\n      \"type\": \"string\",\n      \"description\": \"Depicts mode of payment as mentioned in enum.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-community-pass-payments-validation-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Validation
---
