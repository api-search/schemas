---
description: An hotel booking represent one or several rooms booked in the same physical hotel. There is always a reference to this booking, provided by the hotel provider, stored in associated records section.
layout: schema
name: HotelBooking
properties_list:
- description: Type of data - set to "hotel-booking".
  name: type
  type: string
- description: Unique ID of the hotel booking ID. It is computed by Amadeus System based on technical data.
  name: id
  type: string
- description: 'Status of the booking - Possible values - "CONFIRMED" - "PENDING" for on-request - "CANCELLED" (It will be returned only in the retrieve byHistory as it repreents a DELETED resource.) - "On HOLD" for '
  name: bookingStatus
  type: string
- description: Array of room associations. Each room association correlates one single room to guest(s), a payment and an hotel offer. If multiple identical rooms are requested, one roomAssociation is created per ho
  name: roomAssociations
  type: array
- description: ''
  name: hotelOffer
  type: object
- description: Hotel Content
  name: hotel
  type: object
- description: References and origin of the hotel bookings records
  name: hotelProviderInformation
  type: array
- description: ''
  name: payment
  type: object
- description: Travel Agent ID also called Booking source or IATA number. - When received in booking request, it indicates that the travel agent wants to override the booking source receiving the commission. - If no
  name: travelAgentId
  type: string
- description: Optional information on the way the guest is arriving to the hotel. Today the application only supports Flight details. If this information is provided at booking creation time, it is displayed in the
  name: arrivalInformation
  type: object
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/hotel-booking-hotel-booking-schema.json
slug: hotel-booking-hotel-booking
source_filename: hotel-booking-hotel-booking-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-hotel-booking-schema.json\",\n  \"title\": \"HotelBooking\",\n  \"description\": \"An hotel booking represent one or several rooms booked in the same physical hotel.\\nThere is always a reference to this booking, provided by the hotel provider, stored in associated records section.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"description\": \"Type of data - set to \\\"hotel-booking\\\".\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique ID of the hotel booking ID.\\nIt is computed by Amadeus System based on technical data.\",\n      \"minLength\": 1,\n      \"pattern\": \"[A-Za-z0-9+/=]\",\n      \"example\": \"456123\"\n    },\n    \"bookingStatus\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Status of the booking - Possible values \\n- \\\"CONFIRMED\\\"\\n- \\\"PENDING\\\" for on-request \\n- \\\"CANCELLED\\\" (It will be returned only in the retrieve byHistory as it repreents a DELETED resource.)\\n- \\\"On HOLD\\\" for deferred payment (HO)\\n- \\\"UNCONFIRMED\\\" (UC) when confirmation finaly refused by Hotel Provider\\n- \\\"DENIED\\\" (NO) when an on-request booking is denied by the hotelier\\n- \\\"GHOST\\\" (GK) for ghost booking\\n- \\\"PAST\\\" for a confirmed booking with the check-out date in the past\\n\",\n      \"enum\": [\n        \"CONFIRMED\",\n        \"PENDING\",\n        \"CANCELLED\",\n        \"ON_HOLD\",\n        \"PAST\",\n        \"UNCONFIRMED\",\n        \"DENIED\",\n        \"GHOST\",\n        \"DELETED\"\n      ]\n    },\n    \"roomAssociations\": {\n      \"type\": \"array\",\n      \"description\": \"Array of room associations. Each room association correlates one single room to guest(s), a payment and an\
  \ hotel offer.\\n\\nIf multiple identical rooms are requested, one roomAssociation is created per hotelBooking (one hotelBooking is created per room).\",\n      \"items\": {\n        \"$ref\": \"#/definitions/roomAssociation\"\n      }\n    },\n    \"hotelOffer\": {\n      \"$ref\": \"#/definitions/HotelOffer\"\n    },\n    \"hotel\": {\n      \"type\": \"object\",\n      \"description\": \"Hotel Content\",\n      \"title\": \"Hotel\",\n      \"properties\": {\n        \"hotelId\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z0-9]{8}$\",\n          \"example\": \"ADPAR001\",\n          \"description\": \"Amadeus Property Code (8 chars)\\n\"\n        },\n        \"chainCode\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{2}$\",\n          \"example\": \"AD\",\n          \"description\": \"Brand (RT...) or Merchant (AD...) (Amadeus 2 chars Code)\\n\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Hotel\
  \ de Paris\",\n          \"description\": \"Hotel Name\"\n        },\n        \"self\": {\n          \"type\": \"string\",\n          \"description\": \"link to retrieve the hotel details\"\n        }\n      },\n      \"required\": [\n        \"hotelId\",\n        \"chainCode\",\n        \"name\"\n      ]\n    },\n    \"hotelProviderInformation\": {\n      \"type\": \"array\",\n      \"uniqueItems\": true,\n      \"minItems\": 1,\n      \"description\": \"References and origin of the hotel bookings records\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"hotelProviderCode\": {\n            \"type\": \"string\",\n            \"description\": \"2 letters - Hotel provider code  e.g.RT  (for Accor)\",\n            \"example\": \"RT\",\n            \"minLength\": 2,\n            \"maxLength\": 2\n          },\n          \"confirmationNumber\": {\n            \"type\": \"string\",\n            \"description\": \"Provider confirmation number. \\nNever\
  \ empty, in case of on-request it can be .......\\nIf you call the Provider, this Reference may be asked\",\n            \"example\": \"818319951754\",\n            \"minLength\": 2,\n            \"maxLength\": 16,\n            \"pattern\": \"^[A-Z0-9]*$\"\n          },\n          \"cancellationNumber\": {\n            \"type\": \"string\",\n            \"description\": \"Provider cancellation number\\nFor cancelled booking it will ablways be filled.\\nIf it was not returned by the hotel provider, it will be filled with \\\"NONE\\\".\",\n            \"example\": \"C818319951754\",\n            \"minLength\": 2,\n            \"maxLength\": 16,\n            \"pattern\": \"^[A-Z0-9]*$\"\n          },\n          \"onRequestNumber\": {\n            \"type\": \"string\",\n            \"description\": \"Used to describe the on-request identifier\",\n            \"example\": \"818319951754\",\n            \"minLength\": 2,\n            \"maxLength\": 16,\n            \"pattern\": \"^[A-Z0-9]*$\"\
  \n          }\n        },\n        \"required\": [\n          \"hotelProviderCode\",\n          \"confirmationNumber\"\n        ]\n      }\n    },\n    \"payment\": {\n      \"$ref\": \"#/definitions/PaymentOutput\"\n    },\n    \"travelAgentId\": {\n      \"type\": \"string\",\n      \"description\": \"Travel Agent ID also called Booking source or IATA number.\\n- When received in booking request, it indicates that the travel agent wants to override the booking source receiving the commission. \\n- If not provided in booking request, it is set to the IATA Number of the office profile of the agent making the booking. (the commission is given to that office) \"\n    },\n    \"arrivalInformation\": {\n      \"type\": \"object\",\n      \"description\": \"Optional information on the way the guest is arriving to the hotel. Today the application only supports Flight details.\\nIf this information is provided at booking creation time, it is displayed in the response and in the retrieve.\",\n\
  \      \"properties\": {\n        \"arrivalFlightDetails\": {\n          \"$ref\": \"#/definitions/ArrivalFlightDetails\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"id\",\n    \"roomAssociations\",\n    \"hotelOffer\",\n    \"hotel\",\n    \"hotelProviderInformation\",\n    \"travelAgentId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-hotel-booking-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: HotelBooking
---
