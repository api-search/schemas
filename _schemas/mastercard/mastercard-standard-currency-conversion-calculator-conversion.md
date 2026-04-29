---
description: ''
layout: schema
name: Conversion
properties_list:
- description: Rate applied to the transaction to convert from Transaction Currency to Cardholder Billing Currency.
  name: conversionRate
  type: number
- description: Amount in the cardholder billing currency.
  name: crdhldBillAmt
  type: number
- description: Date of the requested FX rates.
  name: fxDate
  type: string
- description: Currency of the transaction.
  name: transCurr
  type: string
- description: Cardholder billing currency.
  name: crdhldBillCurr
  type: string
- description: Amount in the transaction currency.
  name: transAmt
  type: number
- description: Additional fees imposed by the bank.
  name: bankFee
  type: number
- description: The error code associated with the error being returned.
  name: errorCode
  type: string
- description: The reason for the error.
  name: errorMessage
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-standard-currency-conversion-calculator-conversion-schema.json
slug: mastercard-standard-currency-conversion-calculator-conversion
source_filename: mastercard-standard-currency-conversion-calculator-conversion-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Conversion\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"conversionRate\": {\n      \"type\": \"number\",\n      \"description\": \"Rate applied to the transaction to convert from Transaction Currency to Cardholder Billing Currency.\"\n    },\n    \"crdhldBillAmt\": {\n      \"type\": \"number\",\n      \"description\": \"Amount in the cardholder billing currency.\"\n    },\n    \"fxDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of the requested FX rates.\"\n    },\n    \"transCurr\": {\n      \"type\": \"string\",\n      \"description\": \"Currency of the transaction.\"\n    },\n    \"crdhldBillCurr\": {\n      \"type\": \"string\",\n      \"description\": \"Cardholder billing currency.\"\n    },\n    \"transAmt\": {\n      \"type\": \"number\",\n      \"description\": \"Amount in the transaction currency.\"\n    },\n    \"bankFee\": {\n      \"type\": \"number\"\
  ,\n      \"description\": \"Additional fees imposed by the bank.\"\n    },\n    \"errorCode\": {\n      \"type\": \"string\",\n      \"description\": \"The error code associated with the error being returned.\"\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"The reason for the error.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-standard-currency-conversion-calculator-conversion-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Conversion
---
