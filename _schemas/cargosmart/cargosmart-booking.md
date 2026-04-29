---
description: JSON Schema for a CargoSmart ocean container booking request/confirmation.
layout: schema
name: CargoSmart Container Booking
properties_list:
- description: ''
  name: bookingId
  type: string
- description: Carrier-assigned booking confirmation number
  name: bookingNumber
  type: string
- description: Ocean carrier SCAC code (e.g., MSCU, HLCU, CMDU)
  name: carrierCode
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: originPort
  type: object
- description: ''
  name: destinationPort
  type: object
- description: ''
  name: requestedDepartureDate
  type: string
- description: ''
  name: confirmedVessel
  type: string
- description: ''
  name: confirmedVoyage
  type: string
- description: ''
  name: containers
  type: array
- description: ''
  name: cargoDescription
  type: string
- description: ''
  name: shipper
  type: object
- description: ''
  name: consignee
  type: object
- description: ''
  name: createdAt
  type: string
provider_name: CargoSmart
provider_slug: cargosmart
schema_file: json-schema/cargosmart-booking-schema.json
slug: cargosmart-booking
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cargosmart/refs/heads/main/json-schema/cargosmart-booking-schema.json\",\n  \"title\": \"CargoSmart Container Booking\",\n  \"description\": \"JSON Schema for a CargoSmart ocean container booking request/confirmation.\",\n  \"type\": \"object\",\n  \"required\": [\"bookingId\", \"carrierCode\", \"status\", \"containers\"],\n  \"properties\": {\n    \"bookingId\": {\n      \"type\": \"string\"\n    },\n    \"bookingNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Carrier-assigned booking confirmation number\"\n    },\n    \"carrierCode\": {\n      \"type\": \"string\",\n      \"description\": \"Ocean carrier SCAC code (e.g., MSCU, HLCU, CMDU)\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Submitted\", \"Confirmed\", \"Amended\", \"Cancelled\"]\n    },\n    \"originPort\": {\n      \"$ref\": \"#/$defs/Port\"\
  \n    },\n    \"destinationPort\": {\n      \"$ref\": \"#/$defs/Port\"\n    },\n    \"requestedDepartureDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"confirmedVessel\": {\n      \"type\": \"string\"\n    },\n    \"confirmedVoyage\": {\n      \"type\": \"string\"\n    },\n    \"containers\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"containerType\", \"quantity\"],\n        \"properties\": {\n          \"containerType\": {\n            \"type\": \"string\",\n            \"enum\": [\"20GP\", \"40GP\", \"40HC\", \"20RF\", \"40RF\", \"45HC\"]\n          },\n          \"quantity\": {\n            \"type\": \"integer\",\n            \"minimum\": 1\n          },\n          \"containerId\": {\n            \"type\": \"string\",\n            \"description\": \"Assigned container number (after confirmation)\"\n          }\n        }\n      }\n    },\n    \"cargoDescription\"\
  : {\n      \"type\": \"string\"\n    },\n    \"shipper\": {\n      \"$ref\": \"#/$defs/Party\"\n    },\n    \"consignee\": {\n      \"$ref\": \"#/$defs/Party\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$defs\": {\n    \"Port\": {\n      \"type\": \"object\",\n      \"required\": [\"locode\"],\n      \"properties\": {\n        \"locode\": {\"type\": \"string\", \"pattern\": \"^[A-Z]{5}$\"},\n        \"portName\": {\"type\": \"string\"},\n        \"countryCode\": {\"type\": \"string\", \"pattern\": \"^[A-Z]{2}$\"},\n        \"terminalName\": {\"type\": \"string\"}\n      }\n    },\n    \"Party\": {\n      \"type\": \"object\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\"type\": \"string\"},\n        \"address\": {\"type\": \"string\"},\n        \"city\": {\"type\": \"string\"},\n        \"country\": {\"type\": \"string\"},\n        \"taxId\": {\"type\": \"string\"}\n      }\n    }\n  }\n\
  }\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cargosmart/refs/heads/main/json-schema/cargosmart-booking-schema.json
tags:
- Booking
- Container
- Documentation
- GSBN
- IQAX
- Logistics
- Maritime
- Ocean Freight
- Schedule
- Shipping
- Supply Chain
- Tracking
- Visibility
- Vessel
title: CargoSmart Container Booking
---
