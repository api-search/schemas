---
description: The Payment Methods * CREDIT_CARD (CC) - Payment Cards in `creditCards` are accepted * AGENCY_ACCOUNT - Agency Account (Credit Line) is accepted. Agency is Charged at CheckOut * TRAVEL_AGENT_ID - Agency IATA/ARC Number is accepted to Guarantee the booking * CORPORATE_ID (COR-ID) - Corporate Account is accepted to Guarantee the booking * HOTEL_GUEST_ID - Hotel Chain Rewards Card Number is accepted to Guarantee the booking * CHECK - Checks are accepted * MISC_CHARGE_ORDER - Miscellaneous Charge Order is accepted * ADVANCE_DEPOSIT - Cash is accepted for Deposit/PrePay * COMPANY_ADDRESS - Company Billing Address is accepted to Guarantee the booking
layout: schema
name: Method
properties_list: []
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-method-schema.json
slug: hotel-search-method
source_filename: hotel-search-method-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Method\",\n  \"description\": \"The Payment Methods\\n * CREDIT_CARD (CC) - Payment Cards in `creditCards` are accepted\\n * AGENCY_ACCOUNT - Agency Account (Credit Line) is accepted. Agency is Charged at CheckOut\\n * TRAVEL_AGENT_ID - Agency IATA/ARC Number is accepted to Guarantee the booking\\n * CORPORATE_ID (COR-ID) - Corporate Account is accepted to Guarantee the booking\\n * HOTEL_GUEST_ID - Hotel Chain Rewards Card Number is accepted to Guarantee the booking\\n * CHECK - Checks are accepted\\n * MISC_CHARGE_ORDER - Miscellaneous Charge Order is accepted\\n * ADVANCE_DEPOSIT - Cash is accepted for Deposit/PrePay\\n * COMPANY_ADDRESS - Company Billing Address is accepted to Guarantee the booking\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"CREDIT_CARD\",\n    \"AGENCY_ACCOUNT\",\n    \"TRAVEL_AGENT_ID\",\n    \"CORPORATE_ID\",\n    \"HOTEL_GUEST_ID\",\n    \"CHECK\",\n    \"MISC_CHARGE_ORDER\"\
  ,\n    \"ADVANCE_DEPOSIT\",\n    \"COMPANY_ADDRESS\",\n    \"VCC_BILLBACK\",\n    \"VCC_B2B_WALLET\",\n    \"DEFERED_PAYMENT\",\n    \"TRAVEL_AGENT_IMMEDIATE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-method-schema.json
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
title: Method
---
