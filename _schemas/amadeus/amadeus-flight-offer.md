---
description: A flight offer returned by the Amadeus Flight Offers Search API, representing a purchasable combination of flight segments with pricing for one or more travelers.
layout: schema
name: Amadeus Flight Offer
properties_list:
- description: Resource type identifier for a flight offer.
  name: type
  type: string
- description: Unique identifier for the flight offer within the search results.
  name: id
  type: string
- description: Source of the flight offer data.
  name: source
  type: string
- description: Whether the offer requires immediate ticketing upon booking.
  name: instantTicketingRequired
  type: boolean
- description: Whether the offer contains segments with different booking classes.
  name: nonHomogeneous
  type: boolean
- description: Whether the offer is for a one-way trip.
  name: oneWay
  type: boolean
- description: Last date by which the flight must be ticketed, in ISO 8601 YYYY-MM-DD format.
  name: lastTicketingDate
  type: string
- description: Last date and time by which the flight must be ticketed, in ISO 8601 format.
  name: lastTicketingDateTime
  type: string
- description: Number of seats remaining available for booking on this offer.
  name: numberOfBookableSeats
  type: integer
- description: Array of itineraries composing the trip, each containing one or more flight segments.
  name: itineraries
  type: array
- description: Total price of the flight offer including all travelers.
  name: price
  type: object
- description: Pricing options and fare rules applicable to this offer.
  name: pricingOptions
  type: object
- description: IATA codes of the airlines validating and issuing the tickets.
  name: validatingAirlineCodes
  type: array
- description: Individual pricing breakdown for each traveler on the booking.
  name: travelerPricings
  type: array
- description: Reference dictionaries for codes used in the offer including carriers, aircraft, currencies, and locations.
  name: dictionaries
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/amadeus-flight-offer-schema.json
slug: amadeus-flight-offer
source_filename: amadeus-flight-offer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://amadeus.com/schemas/flight-offer.json\",\n  \"title\": \"Amadeus Flight Offer\",\n  \"description\": \"A flight offer returned by the Amadeus Flight Offers Search API, representing a purchasable combination of flight segments with pricing for one or more travelers.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"type\",\n    \"id\",\n    \"source\",\n    \"itineraries\",\n    \"price\",\n    \"travelerPricings\"\n  ],\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"flight-offer\",\n      \"description\": \"Resource type identifier for a flight offer.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the flight offer within the search results.\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Source of the flight offer data.\",\n      \"enum\": [\"GDS\", \"\
  NDC\", \"LTC\", \"EAC\"]\n    },\n    \"instantTicketingRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the offer requires immediate ticketing upon booking.\"\n    },\n    \"nonHomogeneous\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the offer contains segments with different booking classes.\"\n    },\n    \"oneWay\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the offer is for a one-way trip.\"\n    },\n    \"lastTicketingDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Last date by which the flight must be ticketed, in ISO 8601 YYYY-MM-DD format.\"\n    },\n    \"lastTicketingDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last date and time by which the flight must be ticketed, in ISO 8601 format.\"\n    },\n    \"numberOfBookableSeats\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\"\
  : 9,\n      \"description\": \"Number of seats remaining available for booking on this offer.\"\n    },\n    \"itineraries\": {\n      \"type\": \"array\",\n      \"description\": \"Array of itineraries composing the trip, each containing one or more flight segments.\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/$defs/Itinerary\"\n      }\n    },\n    \"price\": {\n      \"$ref\": \"#/$defs/Price\",\n      \"description\": \"Total price of the flight offer including all travelers.\"\n    },\n    \"pricingOptions\": {\n      \"$ref\": \"#/$defs/PricingOptions\",\n      \"description\": \"Pricing options and fare rules applicable to this offer.\"\n    },\n    \"validatingAirlineCodes\": {\n      \"type\": \"array\",\n      \"description\": \"IATA codes of the airlines validating and issuing the tickets.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^[A-Z0-9]{2}$\"\n      }\n    },\n    \"travelerPricings\": {\n      \"type\": \"array\"\
  ,\n      \"description\": \"Individual pricing breakdown for each traveler on the booking.\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/$defs/TravelerPricing\"\n      }\n    },\n    \"dictionaries\": {\n      \"type\": \"object\",\n      \"description\": \"Reference dictionaries for codes used in the offer including carriers, aircraft, currencies, and locations.\",\n      \"properties\": {\n        \"carriers\": {\n          \"type\": \"object\",\n          \"description\": \"Mapping of airline codes to airline names.\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        },\n        \"aircraft\": {\n          \"type\": \"object\",\n          \"description\": \"Mapping of aircraft codes to aircraft names.\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        },\n        \"currencies\": {\n          \"type\": \"object\",\n          \"description\": \"Mapping of currency codes to currency names.\",\n          \"additionalProperties\"\
  : { \"type\": \"string\" }\n        },\n        \"locations\": {\n          \"type\": \"object\",\n          \"description\": \"Mapping of location codes to location details.\",\n          \"additionalProperties\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"cityCode\": { \"type\": \"string\" },\n              \"countryCode\": { \"type\": \"string\" }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"Itinerary\": {\n      \"type\": \"object\",\n      \"description\": \"A directional journey composed of one or more flight segments.\",\n      \"required\": [\"segments\"],\n      \"properties\": {\n        \"duration\": {\n          \"type\": \"string\",\n          \"description\": \"Total duration of the itinerary in ISO 8601 duration format.\",\n          \"pattern\": \"^PT(\\\\d+H)?(\\\\d+M)?$\"\n        },\n        \"segments\": {\n          \"type\": \"array\",\n          \"description\": \"Individual flight segments\
  \ composing this itinerary.\",\n          \"minItems\": 1,\n          \"items\": {\n            \"$ref\": \"#/$defs/Segment\"\n          }\n        }\n      }\n    },\n    \"Segment\": {\n      \"type\": \"object\",\n      \"description\": \"A single flight leg between two airports.\",\n      \"required\": [\"departure\", \"arrival\", \"carrierCode\", \"number\"],\n      \"properties\": {\n        \"departure\": {\n          \"$ref\": \"#/$defs/FlightEndPoint\",\n          \"description\": \"Departure airport and time information.\"\n        },\n        \"arrival\": {\n          \"$ref\": \"#/$defs/FlightEndPoint\",\n          \"description\": \"Arrival airport and time information.\"\n        },\n        \"carrierCode\": {\n          \"type\": \"string\",\n          \"description\": \"Two-letter IATA airline code of the operating or marketing carrier.\",\n          \"pattern\": \"^[A-Z0-9]{2}$\"\n        },\n        \"number\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Flight number assigned by the carrier.\",\n          \"pattern\": \"^\\\\d{1,4}$\"\n        },\n        \"aircraft\": {\n          \"type\": \"object\",\n          \"description\": \"Aircraft information for this segment.\",\n          \"properties\": {\n            \"code\": {\n              \"type\": \"string\",\n              \"description\": \"IATA aircraft type code.\"\n            }\n          }\n        },\n        \"operating\": {\n          \"type\": \"object\",\n          \"description\": \"Operating carrier information when different from the marketing carrier.\",\n          \"properties\": {\n            \"carrierCode\": {\n              \"type\": \"string\",\n              \"description\": \"IATA code of the operating airline.\",\n              \"pattern\": \"^[A-Z0-9]{2}$\"\n            }\n          }\n        },\n        \"duration\": {\n          \"type\": \"string\",\n          \"description\": \"Duration of this flight segment in ISO 8601 format.\",\n          \"\
  pattern\": \"^PT(\\\\d+H)?(\\\\d+M)?$\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for this segment within the offer.\"\n        },\n        \"numberOfStops\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of technical stops during this segment.\"\n        },\n        \"blacklistedInEU\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the operating carrier is on the EU blacklist.\"\n        }\n      }\n    },\n    \"FlightEndPoint\": {\n      \"type\": \"object\",\n      \"description\": \"Departure or arrival point with airport code, terminal, and time.\",\n      \"required\": [\"iataCode\", \"at\"],\n      \"properties\": {\n        \"iataCode\": {\n          \"type\": \"string\",\n          \"description\": \"Three-letter IATA airport or city code.\",\n          \"pattern\": \"^[A-Z]{3}$\"\n        },\n        \"terminal\": {\n       \
  \   \"type\": \"string\",\n          \"description\": \"Terminal name or number at the airport.\"\n        },\n        \"at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Local date and time of departure or arrival in ISO 8601 format.\"\n        }\n      }\n    },\n    \"Price\": {\n      \"type\": \"object\",\n      \"description\": \"Pricing information for the flight offer.\",\n      \"properties\": {\n        \"currency\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 4217 three-letter currency code.\",\n          \"pattern\": \"^[A-Z]{3}$\"\n        },\n        \"total\": {\n          \"type\": \"string\",\n          \"description\": \"Total price including taxes and fees.\"\n        },\n        \"base\": {\n          \"type\": \"string\",\n          \"description\": \"Base fare amount before taxes and fees.\"\n        },\n        \"fees\": {\n          \"type\": \"array\",\n          \"description\"\
  : \"Breakdown of applicable fees.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"amount\": {\n                \"type\": \"string\",\n                \"description\": \"Fee amount.\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"description\": \"Type of fee.\",\n                \"enum\": [\"SUPPLIER\", \"TICKETING\"]\n              }\n            }\n          }\n        },\n        \"grandTotal\": {\n          \"type\": \"string\",\n          \"description\": \"Final total price including all fees and surcharges.\"\n        },\n        \"additionalServices\": {\n          \"type\": \"array\",\n          \"description\": \"Additional paid services included in the price.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"amount\": { \"type\": \"string\" },\n              \"type\": { \"type\": \"string\" }\n     \
  \       }\n          }\n        }\n      }\n    },\n    \"PricingOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Options controlling how the fare was priced.\",\n      \"properties\": {\n        \"fareType\": {\n          \"type\": \"array\",\n          \"description\": \"Types of fares included in the pricing.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\"PUBLISHED\", \"NEGOTIATED\", \"CORPORATE\"]\n          }\n        },\n        \"includedCheckedBagsOnly\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the price includes only fares with checked baggage.\"\n        }\n      }\n    },\n    \"TravelerPricing\": {\n      \"type\": \"object\",\n      \"description\": \"Pricing breakdown for an individual traveler.\",\n      \"required\": [\"travelerId\", \"fareOption\", \"travelerType\", \"price\"],\n      \"properties\": {\n        \"travelerId\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Identifier of the traveler this pricing applies to.\"\n        },\n        \"fareOption\": {\n          \"type\": \"string\",\n          \"description\": \"Fare option selected for this traveler.\",\n          \"enum\": [\"STANDARD\", \"INCLUSIVE_TOUR\", \"SPANISH_MELILLA_RESIDENT\", \"SPANISH_CEUTA_RESIDENT\", \"SPANISH_CANARY_RESIDENT\", \"SPANISH_BALEARIC_RESIDENT\", \"AIR_FRANCE_METROPOLITAN_DISCOUNT_PASS\", \"AIR_FRANCE_DOM_DISCOUNT_PASS\", \"AIR_FRANCE_COMBINED_DISCOUNT_PASS\", \"AIR_FRANCE_FAMILY\", \"ADULT_WITH_COMPANION\", \"COMPANION\"]\n        },\n        \"travelerType\": {\n          \"type\": \"string\",\n          \"description\": \"Type of traveler for pricing category purposes.\",\n          \"enum\": [\"ADULT\", \"CHILD\", \"SEATED_INFANT\", \"HELD_INFANT\"]\n        },\n        \"price\": {\n          \"$ref\": \"#/$defs/Price\",\n          \"description\": \"Price for this individual traveler.\"\n        },\n        \"fareDetailsBySegment\": {\n          \"type\"\
  : \"array\",\n          \"description\": \"Fare details broken down by each flight segment.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"segmentId\": {\n                \"type\": \"string\",\n                \"description\": \"Reference to the segment this fare applies to.\"\n              },\n              \"cabin\": {\n                \"type\": \"string\",\n                \"description\": \"Cabin class for this segment.\",\n                \"enum\": [\"ECONOMY\", \"PREMIUM_ECONOMY\", \"BUSINESS\", \"FIRST\"]\n              },\n              \"fareBasis\": {\n                \"type\": \"string\",\n                \"description\": \"Fare basis code indicating the fare rules.\"\n              },\n              \"brandedFare\": {\n                \"type\": \"string\",\n                \"description\": \"Name of the branded fare if applicable.\"\n              },\n              \"class\": {\n                \"type\": \"string\"\
  ,\n                \"description\": \"Booking class letter code.\",\n                \"pattern\": \"^[A-Z]$\"\n              },\n              \"includedCheckedBags\": {\n                \"type\": \"object\",\n                \"description\": \"Checked baggage allowance for this segment.\",\n                \"properties\": {\n                  \"weight\": {\n                    \"type\": \"integer\",\n                    \"description\": \"Weight allowance in kilograms.\"\n                  },\n                  \"weightUnit\": {\n                    \"type\": \"string\",\n                    \"description\": \"Unit of weight measurement.\"\n                  },\n                  \"quantity\": {\n                    \"type\": \"integer\",\n                    \"description\": \"Number of bags included.\"\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/amadeus-flight-offer-schema.json
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
title: Amadeus Flight Offer
---
