---
description: Ticketing agreement option * **CONFIRM**, when the payment is done * **DELAY_TO_QUEUE**, queue the reservation at a wished date if the payment is not done * **DELAY_TO_CANCEL**, cancel the reservation at a wished date if the payment is not done Queueing and cancellation occurs at local date and time. When no time is specified, reservation is queued or cancelled at 00:00.
layout: schema
name: TicketingAgreementOption
properties_list: []
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-create-orders-ticketingagreementoption-schema.json
slug: flight-create-orders-ticketingagreementoption
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"TicketingAgreementOption\",\n  \"description\": \"Ticketing agreement option\\n* **CONFIRM**, when the payment is done\\n* **DELAY_TO_QUEUE**, queue the reservation at a wished date if the payment is not done\\n* **DELAY_TO_CANCEL**, cancel the reservation at a wished date if the payment is not done\\n\\nQueueing and cancellation occurs at local date and time. When no time is specified, reservation is queued or cancelled at 00:00.\\n\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"CONFIRM\",\n    \"DELAY_TO_QUEUE\",\n    \"DELAY_TO_CANCEL\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-create-orders-ticketingagreementoption-schema.json
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
title: TicketingAgreementOption
---
