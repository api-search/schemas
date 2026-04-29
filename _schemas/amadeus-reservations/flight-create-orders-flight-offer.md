---
description: FlightOffer schema
layout: schema
name: FlightOffer
properties_list:
- description: the resource name
  name: type
  type: string
- description: Id of the flight offer
  name: id
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
- description: If true, the flight offer can be combined with other oneWays flight-offers to complete the whole journey (one-Way combinable feature).
  name: oneWay
  type: boolean
- description: If true, a payment card is mandatory to book this flight offer
  name: paymentCardRequired
  type: boolean
- description: If booked on the same day as the search (with respect to timezone), this flight offer is guaranteed to be thereafter valid for ticketing until this date (included). Unspecified when it does not make s
  name: lastTicketingDate
  type: string
- description: If booked on the same day as the search (with respect to timezone), this flight offer is guaranteed to be thereafter valid for ticketing until this date/time (included). Unspecified when it does not m
  name: lastTicketingDateTime
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
- description: This option ensures that the system will only consider offers with these airlines as validating carrier.
  name: validatingAirlineCodes
  type: array
- description: Fare information for each traveler/segment
  name: travelerPricings
  type: array
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-flight-offer-schema.json
slug: flight-create-orders-flight-offer
source_filename: flight-create-orders-flight-offer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-flight-offer-schema.json\",\n  \"title\": \"FlightOffer\",\n  \"description\": \"FlightOffer schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"the resource name\",\n      \"example\": \"flight-offer\"\n    },\n    \"id\": {\n      \"description\": \"Id of the flight offer\",\n      \"type\": \"string\",\n      \"example\": \"1\"\n    },\n    \"source\": {\n      \"$ref\": \"#/definitions/FlightOfferSource\"\n    },\n    \"instantTicketingRequired\": {\n      \"description\": \"If true, inform that a ticketing will be required at booking step.\",\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"disablePricing\": {\n      \"description\": \"BOOK step ONLY - If true, allows to book\
  \ a PNR without pricing. Only for the source \\\"GDS\\\"\",\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"nonHomogeneous\": {\n      \"description\": \"If true, upon completion of the booking, this pricing solution is expected to yield multiple records (a record contains booking information confirmed and stored, typically a Passenger Name Record (PNR), in the provider GDS or system)\",\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"oneWay\": {\n      \"description\": \"If true, the flight offer can be combined with other oneWays flight-offers to complete the whole journey (one-Way combinable feature).\",\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"paymentCardRequired\": {\n      \"description\": \"If true, a payment card is mandatory to book this flight offer\",\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"lastTicketingDate\": {\n      \"description\": \"If booked on the same day as the\
  \ search (with respect to timezone), this flight offer is guaranteed to be thereafter valid for ticketing until this date (included). Unspecified when it does not make sense for this flight offer (e.g. no control over ticketing once booked). YYYY-MM-DD format, e.g. 2019-06-07\",\n      \"type\": \"string\",\n      \"example\": \"2018-06-19\"\n    },\n    \"lastTicketingDateTime\": {\n      \"description\": \"If booked on the same day as the search (with respect to timezone), this flight offer is guaranteed to be thereafter valid for ticketing until this date/time (included). Unspecified when it does not make sense for this flight offer (e.g. no control over ticketing once booked). Information only this attribute is not used in input of pricing request. Local date and time in YYYY-MM-ddThh:mm:ss format, e.g. 2017-02-10T20:40:00\",\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2018-06-19T15:00:00\"\n    },\n    \"numberOfBookableSeats\": {\n      \"\
  description\": \"Number of seats bookable in a single request. Can not be higher than 9.\",\n      \"type\": \"number\",\n      \"example\": 9,\n      \"minimum\": 1,\n      \"maximum\": 9\n    },\n    \"itineraries\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"maxItems\": 250,\n      \"items\": {\n        \"title\": \"Itineraries\",\n        \"type\": \"object\",\n        \"properties\": {\n          \"duration\": {\n            \"description\": \"duration in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M for a duration of 2h10m\",\n            \"type\": \"string\",\n            \"example\": \"PT2H10M\"\n          },\n          \"segments\": {\n            \"title\": \"Segments\",\n            \"type\": \"array\",\n            \"minItems\": 1,\n            \"maxItems\": 9,\n            \"items\": {\n              \"$ref\": \"#/definitions/Segment\"\n            }\n          }\n        },\n        \"required\": [\n          \"\
  segments\"\n        ]\n      }\n    },\n    \"price\": {\n      \"$ref\": \"#/definitions/Extended_Price\"\n    },\n    \"pricingOptions\": {\n      \"title\": \"PricingOptions\",\n      \"type\": \"object\",\n      \"properties\": {\n        \"fareType\": {\n          \"description\": \"type of fare of the flight-offer\",\n          \"$ref\": \"#/definitions/PricingOptionsFareType\"\n        },\n        \"includedCheckedBagsOnly\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, returns the flight-offers with included checked bags only\",\n          \"example\": true\n        },\n        \"refundableFare\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, returns the flight-offers with refundable fares only\",\n          \"example\": true\n        },\n        \"noRestrictionFare\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, returns the flight-offers with no restriction fares only\",\n          \"example\"\
  : true\n        },\n        \"noPenaltyFare\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, returns the flight-offers with no penalty fares only\",\n          \"example\": true\n        }\n      }\n    },\n    \"validatingAirlineCodes\": {\n      \"description\": \"This option ensures that the system will only consider offers with these airlines as validating carrier.\",\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"maxItems\": 9,\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"AF\"\n      ]\n    },\n    \"travelerPricings\": {\n      \"title\": \"TravelerPricings\",\n      \"description\": \"Fare information for each traveler/segment\",\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"maxItems\": 18,\n      \"items\": {\n        \"title\": \"TravelerPricing\",\n        \"required\": [\n          \"travelerId\",\n          \"fareOption\",\n          \"travelerType\",\n          \"fareDetailsBySegment\"\
  \n        ],\n        \"properties\": {\n          \"travelerId\": {\n            \"type\": \"string\",\n            \"example\": \"1\",\n            \"description\": \"Id of the traveler\"\n          },\n          \"fareOption\": {\n            \"$ref\": \"#/definitions/TravelerPricingFareOption\"\n          },\n          \"travelerType\": {\n            \"$ref\": \"#/definitions/TravelerType\"\n          },\n          \"associatedAdultId\": {\n            \"type\": \"string\",\n            \"description\": \"if type=\\\"HELD_INFANT\\\", corresponds to the adult traveler's id who will share the seat\"\n          },\n          \"price\": {\n            \"description\": \"price detail of the traveler\",\n            \"$ref\": \"#/definitions/Price\"\n          },\n          \"fareDetailsBySegment\": {\n            \"type\": \"array\",\n            \"minItems\": 1,\n            \"maxItems\": 18,\n            \"items\": {\n              \"title\": \"FareDetailsBySegment\",\n             \
  \ \"description\": \"Fare details of the segment\",\n              \"required\": [\n                \"segmentId\"\n              ],\n              \"properties\": {\n                \"segmentId\": {\n                  \"type\": \"string\",\n                  \"example\": \"1\",\n                  \"description\": \"Id of the segment\"\n                },\n                \"cabin\": {\n                  \"$ref\": \"#/definitions/TravelClass\"\n                },\n                \"fareBasis\": {\n                  \"description\": \"Fare basis specifying the rules of a fare. Usually, though not always, is composed of the booking class code followed by a set of letters and digits representing other characteristics of the ticket, such as refundability, minimum stay requirements, discounts or special promotional elements.\",\n                  \"type\": \"string\",\n                  \"example\": \"ANNNNF4K\",\n                  \"pattern\": \"[[A-Z0-9]{1,18}\"\n                },\n      \
  \          \"brandedFare\": {\n                  \"description\": \"The name of the Fare Family corresponding to the fares. Only for the GDS provider and if the airline has fare families filled\",\n                  \"type\": \"string\",\n                  \"example\": \"LIGHTONE\"\n                },\n                \"class\": {\n                  \"description\": \"The code of the booking class, a.k.a. class of service or Reservations/Booking Designator (RBD)\",\n                  \"type\": \"string\",\n                  \"example\": \"A\",\n                  \"pattern\": \"[A-Z]{1}\"\n                },\n                \"isAllotment\": {\n                  \"description\": \"True if the corresponding booking class is in an allotment\",\n                  \"type\": \"boolean\",\n                  \"example\": true\n                },\n                \"allotmentDetails\": {\n                  \"$ref\": \"#/definitions/AllotmentDetails\"\n                },\n                \"sliceDiceIndicator\"\
  : {\n                  \"$ref\": \"#/definitions/SliceDiceIndicator\"\n                },\n                \"includedCheckedBags\": {\n                  \"title\": \"includedCheckedBags\",\n                  \"$ref\": \"#/definitions/BaggageAllowance\",\n                  \"description\": \"Details of the included checked bags\"\n                },\n                \"additionalServices\": {\n                  \"type\": \"object\",\n                  \"title\": \"AdditionalServicesRequest\",\n                  \"properties\": {\n                    \"chargeableCheckedBags\": {\n                      \"title\": \"chargeableCheckedBags\",\n                      \"description\": \"Details of chargeable checked bags\",\n                      \"$ref\": \"#/definitions/ChargeableCheckdBags\"\n                    },\n                    \"chargeableSeat\": {\n                      \"title\": \"chargeableSeat\",\n                      \"description\": \"Details of chargeable seat\",\n         \
  \             \"$ref\": \"#/definitions/ChargeableSeat\"\n                    },\n                    \"chargeableSeatNumber\": {\n                      \"type\": \"string\",\n                      \"description\": \"DEPRECATED - use the chargeableSeat attribute -  seat number\",\n                      \"example\": \"33D\",\n                      \"pattern\": \"[1-9][0-9]{0,2}[A-Z]?\"\n                    },\n                    \"otherServices\": {\n                      \"type\": \"array\",\n                      \"description\": \"Other services to add\",\n                      \"items\": {\n                        \"$ref\": \"#/definitions/ServiceName\"\n                      },\n                      \"example\": [\n                        \"PRIORITY_BOARDING\"\n                      ]\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-flight-offer-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: FlightOffer
---
