---
description: A priced air itinerary returned from Sabre Bargain Finder Max or re-shop operations
layout: schema
name: Sabre Itinerary
properties_list:
- description: Ranking position in shopping response
  name: sequenceNumber
  type: integer
- description: Flight segments composing the itinerary
  name: airItinerary
  type: object
- description: ''
  name: pricingInfo
  type: object
- description: IATA code of the carrier validating the ticket
  name: validatingCarrier
  type: string
- description: ''
  name: ticketingRequirements
  type: object
provider_name: Sabre
provider_slug: sabre
schema_file: json-schema/sabre-itinerary-schema.json
slug: sabre-itinerary
source_filename: sabre-itinerary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.sabre.com/schemas/itinerary\",\n  \"title\": \"Sabre Itinerary\",\n  \"description\": \"A priced air itinerary returned from Sabre Bargain Finder Max or re-shop operations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sequenceNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Ranking position in shopping response\",\n      \"minimum\": 1\n    },\n    \"airItinerary\": {\n      \"type\": \"object\",\n      \"description\": \"Flight segments composing the itinerary\",\n      \"properties\": {\n        \"directionInd\": {\n          \"type\": \"string\",\n          \"enum\": [\"OneWay\", \"Return\", \"OpenJaw\", \"Circle\"],\n          \"description\": \"Itinerary direction type\"\n        },\n        \"originDestinationOptions\": {\n          \"type\": \"array\",\n          \"description\": \"Each leg of the journey\",\n          \"items\": {\n      \
  \      \"type\": \"object\",\n            \"properties\": {\n              \"flightSegments\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"$ref\": \"#/$defs/FlightSegment\"\n                }\n              },\n              \"elapsedTime\": {\n                \"type\": \"integer\",\n                \"description\": \"Total leg duration in minutes\"\n              },\n              \"stops\": {\n                \"type\": \"integer\",\n                \"minimum\": 0,\n                \"description\": \"Number of stops in this leg\"\n              }\n            }\n          }\n        }\n      },\n      \"required\": [\"directionInd\", \"originDestinationOptions\"]\n    },\n    \"pricingInfo\": {\n      \"$ref\": \"#/$defs/PricingInfo\"\n    },\n    \"validatingCarrier\": {\n      \"type\": \"string\",\n      \"description\": \"IATA code of the carrier validating the ticket\",\n      \"pattern\": \"^[A-Z0-9]{2}$\"\n    },\n    \"ticketingRequirements\"\
  : {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ticketType\": {\n          \"type\": \"string\",\n          \"enum\": [\"eTicket\", \"Paper\"]\n        },\n        \"lastTicketingDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        }\n      }\n    }\n  },\n  \"required\": [\"sequenceNumber\", \"airItinerary\", \"pricingInfo\"],\n  \"$defs\": {\n    \"FlightSegment\": {\n      \"type\": \"object\",\n      \"description\": \"A single flight segment (one takeoff and landing)\",\n      \"properties\": {\n        \"departureAirport\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{3}$\",\n          \"description\": \"IATA departure airport code\"\n        },\n        \"arrivalAirport\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{3}$\",\n          \"description\": \"IATA arrival airport code\"\n        },\n        \"departureDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"\
  date-time\"\n        },\n        \"arrivalDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"marketingAirline\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z0-9]{2}$\",\n          \"description\": \"IATA code of marketing carrier\"\n        },\n        \"operatingAirline\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z0-9]{2}$\",\n          \"description\": \"IATA code of operating carrier\"\n        },\n        \"flightNumber\": {\n          \"type\": \"string\",\n          \"example\": \"AA100\"\n        },\n        \"bookingClass\": {\n          \"type\": \"string\",\n          \"description\": \"Reservation booking designator (RBD)\",\n          \"pattern\": \"^[A-Z]$\"\n        },\n        \"cabinClass\": {\n          \"type\": \"string\",\n          \"enum\": [\"Y\", \"W\", \"C\", \"F\"],\n          \"description\": \"Y=Economy, W=PremiumEconomy, C=Business, F=First\"\n        },\n\
  \        \"equipment\": {\n          \"type\": \"string\",\n          \"description\": \"IATA aircraft equipment type code\",\n          \"example\": \"789\"\n        },\n        \"elapsedTime\": {\n          \"type\": \"integer\",\n          \"description\": \"Segment duration in minutes\"\n        },\n        \"stopQuantity\": {\n          \"type\": \"integer\",\n          \"minimum\": 0\n        },\n        \"fareBasis\": {\n          \"type\": \"string\",\n          \"description\": \"Fare basis code for this segment\"\n        }\n      },\n      \"required\": [\n        \"departureAirport\",\n        \"arrivalAirport\",\n        \"departureDateTime\",\n        \"arrivalDateTime\",\n        \"marketingAirline\",\n        \"flightNumber\",\n        \"bookingClass\"\n      ]\n    },\n    \"PricingInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Total pricing breakdown for the itinerary\",\n      \"properties\": {\n        \"baseFare\": {\n          \"$ref\": \"#/$defs/MonetaryAmount\"\
  \n        },\n        \"totalTaxes\": {\n          \"$ref\": \"#/$defs/MonetaryAmount\"\n        },\n        \"totalFare\": {\n          \"$ref\": \"#/$defs/MonetaryAmount\"\n        },\n        \"taxes\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"taxCode\": {\n                \"type\": \"string\",\n                \"description\": \"IATA tax code (e.g., US, YQ, YR)\"\n              },\n              \"amount\": {\n                \"$ref\": \"#/$defs/MonetaryAmount\"\n              },\n              \"description\": {\n                \"type\": \"string\"\n              }\n            },\n            \"required\": [\"taxCode\", \"amount\"]\n          }\n        },\n        \"passengerTypeBreakdown\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"passengerType\": {\n                \"type\": \"string\"\
  ,\n                \"enum\": [\"ADT\", \"CHD\", \"INF\", \"INS\"]\n              },\n              \"quantity\": {\n                \"type\": \"integer\"\n              },\n              \"perPassengerFare\": {\n                \"$ref\": \"#/$defs/MonetaryAmount\"\n              }\n            }\n          }\n        }\n      },\n      \"required\": [\"baseFare\", \"totalFare\"]\n    },\n    \"MonetaryAmount\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"amount\": {\n          \"type\": \"number\",\n          \"minimum\": 0\n        },\n        \"currencyCode\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{3}$\",\n          \"description\": \"ISO 4217 currency code\"\n        }\n      },\n      \"required\": [\"amount\", \"currencyCode\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sabre/refs/heads/main/json-schema/sabre-itinerary-schema.json
tags:
- Travel
- GDS
- Airlines
- Hotels
- Car Rental
- Booking
title: Sabre Itinerary
---
