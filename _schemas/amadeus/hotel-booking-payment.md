---
description: form of payment (mandatory in case of `acceptedPayments`/`methods`)
layout: schema
name: Payment
properties_list:
- description: ''
  name: id
  type: integer
- description: 'The Payment Methods: * creditCard (CC) - Payment Cards in `creditCards` are accepted'
  name: method
  type: string
- description: payment card details (mandatory in case of `method` creditCard)
  name: card
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-booking-payment-schema.json
slug: hotel-booking-payment
source_filename: hotel-booking-payment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Payment\",\n  \"description\": \"form of payment (mandatory in case of `acceptedPayments`/`methods`)\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"method\": {\n      \"type\": \"string\",\n      \"description\": \"The Payment Methods:\\n * creditCard (CC) - Payment Cards in `creditCards` are accepted           \",\n      \"enum\": [\n        \"creditCard\"\n      ]\n    },\n    \"card\": {\n      \"type\": \"object\",\n      \"description\": \"payment card details (mandatory in case of `method` creditCard)\",\n      \"properties\": {\n        \"vendorCode\": {\n          \"type\": \"string\",\n          \"description\": \"card type (CA, VI, AX, DC...)\\nExamples:\\n  * CA - MasterCard (warning: use it instead of MC/IK/EC/MD/XS)\\n  * VI - Visa\\n  * AX - American Express\\n  * DC - Diners Club\\n  * AU - Carte Aurore\\n  * CG - Cofinoga\\\
  n  * DS - Discover\\n  * GK - Lufthansa GK Card\\n  * JC - Japanese Credit Bureau\\n  * TC - Torch Club\\n  * TP - Universal Air Travel Card\\n  * BC - Bank Card\\n  * DL - Delta\\n  * MA - Maestro\\n  * UP - China UnionPay   \\n  * VE - Visa Electron\\n\"\n        },\n        \"cardNumber\": {\n          \"type\": \"string\",\n          \"description\": \"card number\"\n        },\n        \"expiryDate\": {\n          \"type\": \"string\",\n          \"description\": \"Expiration Date YYYY-MM\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"method\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-booking-payment-schema.json
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
title: Payment
---
