---
description: ''
layout: schema
name: Transfer
properties_list:
- description: amadeus transfer service type value | description -- | PRIVATE | Private transfer from point to point SHARED | Shared transfer from point to point TAXI | Taxi reservation from point to point, price is
  name: transferType
  type: string
- description: ''
  name: start
  type: object
- description: ''
  name: end
  type: object
- description: ''
  name: stopOvers
  type: array
- description: ''
  name: passenegerCharacteristics
  type: array
- description: transfer duration in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M
  name: duration
  type: string
- description: ''
  name: vehicle
  type: object
- description: ''
  name: serviceProvider
  type: object
- description: ''
  name: partnerInfo
  type: object
- description: ''
  name: quotation
  type: object
- description: ''
  name: converted
  type: object
- description: ''
  name: extraServices
  type: array
- description: ''
  name: equipment
  type: array
- description: ''
  name: cancellationRules
  type: array
- description: list of payment methods, allowed by provider
  name: methodsOfPaymentAccepted
  type: array
- description: list of discount codes
  name: discountCodes
  type: array
- description: ''
  name: distance
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-booking-transfer-schema.json
slug: transfer-booking-transfer
source_filename: transfer-booking-transfer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Transfer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transferType\": {\n      \"type\": \"string\",\n      \"description\": \"amadeus transfer service type\\n\\nvalue           | description                                 \\n--  | \\nPRIVATE         | Private transfer from point to point\\nSHARED          | Shared transfer from point to point\\nTAXI            | Taxi reservation from point to point, price is estimated\\nHOURLY          | Chauffeured driven transfer per hour\\nAIRPORT_EXPRESS | Express Train from/to Airport\\nAIRPORT_BUS     | Express Bus from/to Airport\\nHELICOPTER      | Private helicopter flight from/to airport\\nPRIVATE_JET     | Private flight from airport to airport\\n\",\n      \"enum\": [\n        \"PRIVATE\",\n        \"SHARED\",\n        \"TAXI\",\n        \"HOURLY\",\n        \"AIRPORT_EXPRESS\",\n        \"HELICOPTER\",\n        \"PRIVATE_JET\",\n       \
  \ \"AIRPORT_BUS\"\n      ]\n    },\n    \"start\": {\n      \"$ref\": \"#/definitions/Location\"\n    },\n    \"end\": {\n      \"$ref\": \"#/definitions/Location\"\n    },\n    \"stopOvers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/StopOver\"\n      }\n    },\n    \"passenegerCharacteristics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/PassengerCharacteristics\"\n      }\n    },\n    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"transfer duration in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M\"\n    },\n    \"vehicle\": {\n      \"$ref\": \"#/definitions/Vehicle\"\n    },\n    \"serviceProvider\": {\n      \"$ref\": \"#/definitions/ServiceProvider\"\n    },\n    \"partnerInfo\": {\n      \"$ref\": \"#/definitions/PartnerInfo\"\n    },\n    \"quotation\": {\n      \"$ref\": \"#/definitions/Quotation\"\n    },\n    \"converted\": {\n\
  \      \"$ref\": \"#/definitions/Quotation\"\n    },\n    \"extraServices\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/ExtraService\"\n      }\n    },\n    \"equipment\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Equipment\"\n      }\n    },\n    \"cancellationRules\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/CancellationRule\"\n      }\n    },\n    \"methodsOfPaymentAccepted\": {\n      \"type\": \"array\",\n      \"description\": \"list of payment methods, allowed by provider\",\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"Method of payment required when PaymentType equal BT (applicable only for reservation action).\",\n        \"enum\": [\n          \"CREDIT_CARD\",\n          \"INVOICE\",\n          \"TRAVEL_ACCOUNT\",\n          \"PAYMENT_SERVICE_PROVIDER\"\n        ]\n      }\n    },\n    \"discountCodes\": {\n      \"\
  type\": \"array\",\n      \"description\": \"list of discount codes\",\n      \"items\": {\n        \"$ref\": \"#/definitions/DiscountCode\"\n      }\n    },\n    \"distance\": {\n      \"$ref\": \"#/definitions/Distance\"\n    }\n  },\n  \"required\": [\n    \"transferType\",\n    \"start\",\n    \"serviceProvider\",\n    \"vehicle\",\n    \"quotation\",\n    \"methodsOfPaymentAccepted\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/transfer-booking-transfer-schema.json
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
title: Transfer
---
