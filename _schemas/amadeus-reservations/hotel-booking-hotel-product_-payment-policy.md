---
description: Accepted Payment Methods and Card Types. Several Payment Methods and Card Types may be available.
layout: schema
name: HotelProduct_PaymentPolicy
properties_list:
- description: Accepted Payment Card Types for the `method` CREDIT_CARD
  name: creditCards
  type: array
- description: Accepted Payment Methods
  name: methods
  type: array
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/hotel-booking-hotel-product_-payment-policy-schema.json
slug: hotel-booking-hotel-product_-payment-policy
source_filename: hotel-booking-hotel-product_-payment-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-hotel-product_-payment-policy-schema.json\",\n  \"title\": \"HotelProduct_PaymentPolicy\",\n  \"description\": \"Accepted Payment Methods and Card Types. Several Payment Methods and Card Types may be available.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"creditCards\": {\n      \"type\": \"array\",\n      \"description\": \"Accepted Payment Card Types for the `method` CREDIT_CARD\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^[A-Z]{2}$\",\n        \"minLength\": 2,\n        \"maxLength\": 2,\n        \"example\": \"VI\",\n        \"description\": \"card type (CA, VI, AX, DC...)\\nExamples:\\n  * CA - Mastercard (warning: use it instead of MC/IK/EC/MD/XS)\\n  * VI - VISA\\n  * AX - AMERICAN EXPRESS\\n  * DC - Diners Club\\n  * DS - DISCOVER\\\
  n  * JC - JCB\\n  * TP - UATP / AirPlus\\n  * UP - UnionPay  \\n\"\n      },\n      \"example\": [\n        \"CA\",\n        \"VI\",\n        \"AX\"\n      ]\n    },\n    \"methods\": {\n      \"type\": \"array\",\n      \"description\": \"Accepted Payment Methods\",\n      \"items\": {\n        \"type\": \"string\",\n        \"example\": \"CREDIT_CARD\",\n        \"enum\": [\n          \"CREDIT_CARD\",\n          \"CREDIT_CARD_AGENCY\",\n          \"CREDIT_CARD_TRAVELER\",\n          \"VCC_BILLBACK\",\n          \"VCC_B2B_WALLET\",\n          \"TRAVEL_AGENT_ID\",\n          \"AGENCY_ACCOUNT\",\n          \"CORPORATE_ID\",\n          \"CHECK\",\n          \"ADVANCE_DEPOSIT\",\n          \"COMPANY_ADDRESS\",\n          \"HOTEL_GUEST_ID\",\n          \"MISC_CHARGE_ORDER\",\n          \"DEFERED_PAYMENT\",\n          \"TRAVEL_AGENT_IMMEDIATE\"\n        ],\n        \"description\": \"The Payment Methods :\\n * CREDIT_CARD (CC) - Payment Cards in `creditCards` are accepted\\n * CREDIT_CARD_AGENCY\
  \ (CA) - Payment Cards in `creditCards` are accepted\\n * CREDIT_CARD_TRAVELER (CC) - Payment Cards in `creditCards` are accepted\\n * AGENCY_ACCOUNT - Agency Account (Credit Line) is accepted. Agency is Charged at CheckOut\\n * TRAVEL_AGENT_ID - Agency IATA/ARC Number is accepted to Guarantee the booking\\n * CORPORATE_ID (COR-ID) - Corporate Account is accepted to Guarantee the booking\\n * HOTEL_GUEST_ID - Hotel Chain Rewards Card Number is accepted to Guarantee the booking\\n * CHECK - Checks are accepted\\n * MISC_CHARGE_ORDER - Miscellaneous Charge Order is accepted\\n * ADVANCE_DEPOSIT - Cash is accepted for Deposit/PrePay\\n * COMPANY_ADDRESS - Company Billing Address is accepted to Guarantee the booking\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-hotel-product_-payment-policy-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: HotelProduct_PaymentPolicy
---
