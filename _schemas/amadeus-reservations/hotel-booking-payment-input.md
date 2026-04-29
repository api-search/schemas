---
description: Model with the hotel payment information
layout: schema
name: PaymentInput
properties_list:
- description: Agency IATA/ARC Number used to Guarantee the booking. If not provided it is taken form the Amadeus Office profile.
  name: iataTravelAgency
  type: object
- description: 'Indicates the method of payment. - CREDIT_CARD : It allows payment through a credit card. It is expected to provide the credit card information in the paymentCard section.'
  name: method
  type: string
- description: 'Credit card information. The full details of a credit card are expected : . credit card holder name (mandatory, maximum 64 chars) . credit card vendor code (mandatory) . credit card number (mandatory)'
  name: paymentCard
  type: object
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/hotel-booking-payment-input-schema.json
slug: hotel-booking-payment-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-payment-input-schema.json\",\n  \"title\": \"PaymentInput\",\n  \"description\": \"Model with the hotel payment information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"iataTravelAgency\": {\n      \"type\": \"object\",\n      \"description\": \"Agency IATA/ARC Number used to Guarantee the booking.\\nIf not provided it is taken form the Amadeus Office profile.\",\n      \"properties\": {\n        \"iataNumber\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"method\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates the method of payment. \\n- CREDIT_CARD : It allows payment through a credit card. It is expected to provide the credit card information in the paymentCard section.\",\n      \"enum\": [\n        \"CREDIT_CARD\"\n      ]\n\
  \    },\n    \"paymentCard\": {\n      \"type\": \"object\",\n      \"description\": \"Credit card information.\\nThe full details of a credit card are expected :\\n  . credit card holder name (mandatory, maximum 64 chars) \\n  . credit card vendor code (mandatory)\\n  . credit card number (mandatory)\\n  . credit card expiry date (mandatory)\\n  . credit card security code (optional, it is anyway strongly recommended to always provide it for Aggregators)\",\n      \"properties\": {\n        \"paymentCardInfo\": {\n          \"type\": \"object\",\n          \"description\": \"Credit or Debits cards.\",\n          \"title\": \"PaymentCard\",\n          \"properties\": {\n            \"vendorCode\": {\n              \"type\": \"string\",\n              \"example\": \"VI\",\n              \"description\": \"Two-letter code card type or vendor code. E.g. VI for VISA, MA for MasterCard.\",\n              \"maxLength\": 30,\n              \"minLength\": 0\n            },\n            \"holderName\"\
  : {\n              \"type\": \"string\",\n              \"description\": \"Name of credit card holder.\",\n              \"maxLength\": 99,\n              \"minLength\": 1\n            },\n            \"cardNumber\": {\n              \"type\": \"string\",\n              \"description\": \"Card number\"\n            },\n            \"securityCode\": {\n              \"type\": \"string\",\n              \"description\": \"Card security code\",\n              \"example\": \"193\",\n              \"minLength\": 3,\n              \"maxLength\": 4\n            },\n            \"expiryDate\": {\n              \"type\": \"string\",\n              \"description\": \"Date of the expiration of the card in the format MMYY\"\n            }\n          },\n          \"required\": [\n            \"vendorCode\",\n            \"holderName\",\n            \"cardNumber\",\n            \"expiryDate\"\n          ]\n        },\n        \"address\": {\n          \"$ref\": \"#/definitions/Address\"\n        }\n\
  \      },\n      \"required\": [\n        \"paymentCardInfo\"\n      ]\n    }\n  },\n  \"required\": [\n    \"method\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-payment-input-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: PaymentInput
---
