---
description: ''
layout: schema
name: AvailabilityClass
properties_list:
- description: Number of seats bookable in a single request. Can not be higher than 9.
  name: numberOfBookableSeats
  type: number
- description: The code of the booking class, a.k.a. class of service or Reservations/Booking Designator (RBD)
  name: class
  type: string
- description: Status of the booking class when it is closed.
  name: closedStatus
  type: string
- description: ''
  name: tourAllotment
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-availibilities-search-availabilityclass-schema.json
slug: flight-availibilities-search-availabilityclass
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"AvailabilityClass\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"numberOfBookableSeats\": {\n      \"type\": \"number\",\n      \"description\": \"Number of seats bookable in a single request. Can not be higher than 9.\"\n    },\n    \"class\": {\n      \"type\": \"string\",\n      \"description\": \"The code of the booking class, a.k.a. class of service or Reservations/Booking Designator (RBD)\"\n    },\n    \"closedStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the booking class when it is closed.\",\n      \"enum\": [\n        \"WAITLIST_OPEN\",\n        \"WAITLIST_CLOSED\",\n        \"ON_REQUEST\"\n      ]\n    },\n    \"tourAllotment\": {\n      \"$ref\": \"#/definitions/TourAllotment\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-availibilities-search-availabilityclass-schema.json
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
title: AvailabilityClass
---
