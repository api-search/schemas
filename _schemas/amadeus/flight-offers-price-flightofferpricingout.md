---
description: priced flight Offers and conditions
layout: schema
name: FlightOfferPricingOut
properties_list:
- description: the resource name
  name: type
  type: string
- description: list of flight offer to price
  name: flightOffers
  type: array
- description: pricing condition at booking level
  name: bookingRequirements
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-price-flightofferpricingout-schema.json
slug: flight-offers-price-flightofferpricingout
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"FlightOfferPricingOut\",\n  \"description\": \"priced flight Offers and conditions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"the resource name\"\n    },\n    \"flightOffers\": {\n      \"type\": \"array\",\n      \"description\": \"list of flight offer to price\",\n      \"items\": {\n        \"$ref\": \"#/definitions/FlightOffer\"\n      }\n    },\n    \"bookingRequirements\": {\n      \"type\": \"object\",\n      \"description\": \"pricing condition at booking level\",\n      \"properties\": {\n        \"invoiceAddressRequired\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, an invoice address is required for the creation of the flight-order\"\n        },\n        \"mailingAddressRequired\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, a postal address is required\
  \ for the creation of the flight-order\"\n        },\n        \"emailAddressRequired\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, an email address is required for the creation of the flight-order\"\n        },\n        \"phoneCountryCodeRequired\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, the phone country code (e.g. '33') associated for each phone number is required for the creation of the flight-order\"\n        },\n        \"mobilePhoneNumberRequired\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, a mobile phone number is required for the creation of the flight-order\"\n        },\n        \"phoneNumberRequired\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, a phone number is required for the creation of the flight-order\"\n        },\n        \"postalCodeRequired\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, a postal code is\
  \ required for the creation of the flight-order\"\n        },\n        \"travelerRequirements\": {\n          \"type\": \"array\",\n          \"description\": \"traveler pricing condition\",\n          \"items\": {\n            \"properties\": {\n              \"travelerId\": {\n                \"type\": \"string\",\n                \"description\": \"Id of the traveler\"\n              },\n              \"genderRequired\": {\n                \"type\": \"boolean\",\n                \"description\": \"If true, the gender is required for the concerned traveler for the creation of the flight-order\"\n              },\n              \"documentRequired\": {\n                \"type\": \"boolean\",\n                \"description\": \"If true, a document is required for the concerned traveler for the creation of the flight-order\"\n              },\n              \"documentIssuanceCityRequired\": {\n                \"type\": \"boolean\",\n                \"description\": \"If true, the isuance\
  \ city of the document is required for the concerned traveler for the creation of the flight-order\"\n              },\n              \"dateOfBirthRequired\": {\n                \"type\": \"boolean\",\n                \"description\": \"If true, the date of bitrth is required for the concerned traveler for the creation of the flight-order\"\n              },\n              \"redressRequiredIfAny\": {\n                \"type\": \"boolean\",\n                \"description\": \"If true, the redress is required if any for the concerned traveler for the creation of the flight-order\"\n              },\n              \"airFranceDiscountRequired\": {\n                \"type\": \"boolean\",\n                \"description\": \"If true, the Air France discount is required for the concerned traveler for the creation of the flight-order\"\n              },\n              \"spanishResidentDiscountRequired\": {\n                \"type\": \"boolean\",\n                \"description\": \"If true, the\
  \ Spanish resident discount is required for the concerned traveler for the creation of the flight-order\"\n              },\n              \"residenceRequired\": {\n                \"type\": \"boolean\",\n                \"description\": \"If true, the address is required for the concerned traveler for the creation of the flight-order\"\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"flightOffers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-offers-price-flightofferpricingout-schema.json
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
title: FlightOfferPricingOut
---
