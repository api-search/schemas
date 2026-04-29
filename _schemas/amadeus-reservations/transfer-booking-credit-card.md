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
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-credit-card-schema.json
slug: transfer-booking-credit-card
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-credit-card-schema.json\",\n  \"title\": \"CreditCard\",\n  \"description\": \"information about payment card\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"number\": {\n      \"type\": \"string\",\n      \"pattern\": \"[0-9]{16}\",\n      \"description\": \"card number\"\n    },\n    \"holderName\": {\n      \"type\": \"string\",\n      \"description\": \"card holder name\"\n    },\n    \"vendorCode\": {\n      \"type\": \"string\",\n      \"pattern\": \"[a-zA-Z]{2}\",\n      \"description\": \"card vendor code, e.g VI \\u2013 VISA, CA \\u2013 MasterCard, AX \\u2013 American Express etc\"\n    },\n    \"expiryDate\": {\n      \"type\": \"string\",\n      \"pattern\": \"^(0[1-9]|1[0-2])[0-9]{2}$\",\n      \"description\": \"card expiry date in format MMYY, e.g. 0237 for February\
  \ 2037\"\n    },\n    \"cvv\": {\n      \"type\": \"string\",\n      \"pattern\": \"[a-zA-Z0-9]{3,4}\",\n      \"description\": \"cerification calue number, as indicated on the credit card. Only for query\"\n    }\n  },\n  \"required\": [\n    \"number\",\n    \"holderName\",\n    \"vendorCode\",\n    \"expiryDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-credit-card-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: CreditCard
---
