---
description: information about payment card
layout: schema
name: CreditCard
properties_list:
- description: card number
  name: number
  type: string
- description: card holder name
  name: holderName
  type: string
- description: card vendor code, e.g VI – VISA, CA – MasterCard, AX – American Express etc
  name: vendorCode
  type: string
- description: card expiry date in format MMYY, e.g. 0237 for February 2037
  name: expiryDate
  type: string
- description: cerification calue number, as indicated on the credit card. Only for query
  name: cvv
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-booking-creditcard-schema.json
slug: transfer-booking-creditcard
source_filename: transfer-booking-creditcard-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreditCard\",\n  \"description\": \"information about payment card\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"card number\"\n    },\n    \"holderName\": {\n      \"type\": \"string\",\n      \"description\": \"card holder name\"\n    },\n    \"vendorCode\": {\n      \"type\": \"string\",\n      \"description\": \"card vendor code, e.g VI \\u2013 VISA, CA \\u2013 MasterCard, AX \\u2013 American Express etc\"\n    },\n    \"expiryDate\": {\n      \"type\": \"string\",\n      \"description\": \"card expiry date in format MMYY, e.g. 0237 for February 2037\"\n    },\n    \"cvv\": {\n      \"type\": \"string\",\n      \"description\": \"cerification calue number, as indicated on the credit card. Only for query\"\n    }\n  },\n  \"required\": [\n    \"number\",\n    \"holderName\",\n    \"vendorCode\",\n    \"expiryDate\"\n\
  \  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/transfer-booking-creditcard-schema.json
tags:
- Airlines
- Aviation
- Booking
- Destinations
- Flights
- Hospitality
- Hotels
- Market Insights
- Tourism
- Transfers
- Travel
title: CreditCard
---
