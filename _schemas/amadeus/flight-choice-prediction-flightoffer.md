---
description: ''
layout: schema
name: FlightOffer
properties_list:
- description: the resource name
  name: type
  type: string
- description: Id of the flight offer
  name: id
  type: string
- description: the choice probability of this Flight Offer. The value is between 1 (100% chance the FlightOffer will be selected) and 0 (no change the FlightOffer will be selected)
  name: choiceProbability
  type: string
- description: ''
  name: source
  type: object
- description: If true, inform that a ticketing will be required at booking step.
  name: instantTicketingRequired
  type: boolean
- description: BOOK step ONLY - If true, allows to book a PNR without pricing. Only for the source "GDS"
  name: disablePricing
  type: boolean
- description: If true, upon completion of the booking, this pricing solution is expected to yield multiple records (a record contains booking information confirmed and stored, typically a Passenger Name Record (PNR
  name: nonHomogeneous
  type: boolean
- description: If true, the flight offer fulfills only one originDestination and has to be combined with other oneWays to complete the whole journey.
  name: oneWay
  type: boolean
- description: If true, a payment card is mandatory to book this flight offer
  name: paymentCardRequired
  type: boolean
- description: If booked on the same day as the search (with respect to timezone), this flight offer is guaranteed to be thereafter valid for ticketing until this date (included). Unspecified when it does not make s
  name: lastTicketingDate
  type: string
- description: Number of seats bookable in a single request. Can not be higher than 9.
  name: numberOfBookableSeats
  type: number
- description: ''
  name: itineraries
  type: array
- description: ''
  name: price
  type: object
- description: ''
  name: pricingOptions
  type: object
- description: This option ensures that the system will only consider these airlines.
  name: validatingAirlineCodes
  type: array
- description: Fare information for each traveler/segment
  name: travelerPricings
  type: array
- description: ''
  name: fareRules
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-choice-prediction-flightoffer-schema.json
slug: flight-choice-prediction-flightoffer
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"FlightOffer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"the resource name\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Id of the flight offer\"\n    },\n    \"choiceProbability\": {\n      \"type\": \"string\",\n      \"description\": \"the choice probability of this Flight Offer. The value is between 1 (100% chance the FlightOffer will be selected) and 0 (no change the FlightOffer will be selected)\"\n    },\n    \"source\": {\n      \"$ref\": \"#/definitions/FlightOfferSource\"\n    },\n    \"instantTicketingRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, inform that a ticketing will be required at booking step.\"\n    },\n    \"disablePricing\": {\n      \"type\": \"boolean\",\n      \"description\": \"BOOK step ONLY - If true, allows to book a PNR without\
  \ pricing. Only for the source \\\"GDS\\\"\"\n    },\n    \"nonHomogeneous\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, upon completion of the booking, this pricing solution is expected to yield multiple records (a record contains booking information confirmed and stored, typically a Passenger Name Record (PNR), in the provider GDS or system)\"\n    },\n    \"oneWay\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, the flight offer fulfills only one originDestination and has to be combined with other oneWays to complete the whole journey.\"\n    },\n    \"paymentCardRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, a payment card is mandatory to book this flight offer\"\n    },\n    \"lastTicketingDate\": {\n      \"type\": \"string\",\n      \"description\": \"If booked on the same day as the search (with respect to timezone), this flight offer is guaranteed to be thereafter valid for ticketing until this date (included).\
  \ Unspecified when it does not make sense for this flight offer (e.g. no control over ticketing once booked). YYYY-MM-DD format, e.g. 2019-06-07\"\n    },\n    \"numberOfBookableSeats\": {\n      \"type\": \"number\",\n      \"description\": \"Number of seats bookable in a single request. Can not be higher than 9.\"\n    },\n    \"itineraries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"duration\": {\n            \"type\": \"string\",\n            \"description\": \"duration in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M for a duration of 2h10m\"\n          },\n          \"segments\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/definitions/Segment\"\n            }\n          }\n        }\n      }\n    },\n    \"price\": {\n      \"$ref\": \"#/definitions/Extended_Price\"\n    },\n    \"pricingOptions\": {\n      \"type\"\
  : \"object\",\n      \"properties\": {\n        \"fareType\": {\n          \"$ref\": \"#/definitions/PricingOptionsFareType\"\n        },\n        \"corporateCodes\": {\n          \"type\": \"array\",\n          \"description\": \"Allow Corporate negotiated fares using one or more corporate number (corporate code).\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"includedCheckedBagsOnly\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, returns the flight-offers with included checked bags only\"\n        },\n        \"refundableFare\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, returns the flight-offers with refundable fares only\"\n        },\n        \"noRestrictionFare\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, returns the flight-offers with no restriction fares only\"\n        },\n        \"noPenaltyFare\": {\n          \"type\": \"boolean\"\
  ,\n          \"description\": \"If true, returns the flight-offers with no penalty fares only\"\n        }\n      }\n    },\n    \"validatingAirlineCodes\": {\n      \"type\": \"array\",\n      \"description\": \"This option ensures that the system will only consider these airlines.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"travelerPricings\": {\n      \"type\": \"array\",\n      \"description\": \"Fare information for each traveler/segment\",\n      \"items\": {\n        \"properties\": {\n          \"travelerId\": {\n            \"type\": \"string\",\n            \"description\": \"Id of the traveler\"\n          },\n          \"fareOption\": {\n            \"$ref\": \"#/definitions/TravelerPricingFareOption\"\n          },\n          \"travelerType\": {\n            \"$ref\": \"#/definitions/TravelerType\"\n          },\n          \"associatedAdultId\": {\n            \"type\": \"string\",\n            \"description\": \"if type=\\\"HELD_INFANT\\\"\
  , corresponds to the adult traveler's id who will share the seat\"\n          },\n          \"price\": {\n            \"$ref\": \"#/definitions/Price\"\n          },\n          \"fareDetailsBySegment\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"description\": \"Fare details of the segment\",\n              \"properties\": {\n                \"segmentId\": {\n                  \"type\": \"string\",\n                  \"description\": \"Id of the segment\"\n                },\n                \"cabin\": {\n                  \"$ref\": \"#/definitions/TravelClass\"\n                },\n                \"fareBasis\": {\n                  \"type\": \"string\",\n                  \"description\": \"Fare basis specifying the rules of a fare. Usually, though not always, is composed of the booking class code followed by a set of letters and digits representing other characteristics of the ticket, such as refundability, minimum stay requirements, discounts or\
  \ special promotional elements.\"\n                },\n                \"brandedFare\": {\n                  \"type\": \"string\",\n                  \"description\": \"The name of the Fare Family corresponding to the fares. Only for the GDS provider and if the airline has fare families filled\"\n                },\n                \"class\": {\n                  \"type\": \"string\",\n                  \"description\": \"The code of the booking class, a.k.a. class of service or Reservations/Booking Designator (RBD)\"\n                },\n                \"isAllotment\": {\n                  \"type\": \"boolean\",\n                  \"description\": \"True if the corresponding booking class is in an allotment\"\n                },\n                \"allotmentDetails\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"tourName\": {\n                      \"type\": \"string\"\n                    },\n                    \"tourReference\"\
  : {\n                      \"type\": \"string\"\n                    }\n                  }\n                },\n                \"sliceDiceIndicator\": {\n                  \"$ref\": \"#/definitions/SliceDiceIndicator\"\n                },\n                \"includedCheckedBags\": {\n                  \"$ref\": \"#/definitions/BaggageAllowance\"\n                },\n                \"additionalServices\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"chargeableCheckedBags\": {\n                      \"$ref\": \"#/definitions/BaggageAllowance\"\n                    },\n                    \"chargeableSeatNumber\": {\n                      \"type\": \"string\",\n                      \"description\": \"seat number\"\n                    },\n                    \"otherServices\": {\n                      \"type\": \"array\",\n                      \"description\": \"Other services to add\",\n                      \"items\": {\n   \
  \                     \"$ref\": \"#/definitions/ServiceName\"\n                      }\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"fareRules\": {\n      \"$ref\": \"#/definitions/FareRules\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"id\",\n    \"source\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-choice-prediction-flightoffer-schema.json
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
title: FlightOffer
---
