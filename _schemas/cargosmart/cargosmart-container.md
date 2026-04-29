---
description: JSON Schema for a CargoSmart container tracking record including event history and vessel information.
layout: schema
name: CargoSmart Container Tracking
properties_list:
- description: ISO 6346 container number (e.g., MSCU1234567)
  name: containerId
  type: string
- description: ISO container type code
  name: containerType
  type: string
- description: Ocean carrier SCAC code
  name: carrierCode
  type: string
- description: ''
  name: vesselName
  type: string
- description: ''
  name: voyageNumber
  type: string
- description: ''
  name: currentStatus
  type: string
- description: ''
  name: originPort
  type: object
- description: ''
  name: destinationPort
  type: object
- description: Estimated arrival at destination port
  name: estimatedArrival
  type: string
- description: Actual arrival at destination port
  name: actualArrival
  type: string
- description: Chronological list of tracking events
  name: events
  type: array
- description: ''
  name: lastUpdated
  type: string
provider_name: CargoSmart
provider_slug: cargosmart
schema_file: json-schema/cargosmart-container-schema.json
slug: cargosmart-container
source_filename: cargosmart-container-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cargosmart/refs/heads/main/json-schema/cargosmart-container-schema.json\",\n  \"title\": \"CargoSmart Container Tracking\",\n  \"description\": \"JSON Schema for a CargoSmart container tracking record including event history and vessel information.\",\n  \"type\": \"object\",\n  \"required\": [\"containerId\", \"currentStatus\"],\n  \"properties\": {\n    \"containerId\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 6346 container number (e.g., MSCU1234567)\",\n      \"pattern\": \"^[A-Z]{4}\\\\d{7}$\"\n    },\n    \"containerType\": {\n      \"type\": \"string\",\n      \"description\": \"ISO container type code\",\n      \"enum\": [\"20GP\", \"40GP\", \"40HC\", \"20RF\", \"40RF\", \"45HC\"]\n    },\n    \"carrierCode\": {\n      \"type\": \"string\",\n      \"description\": \"Ocean carrier SCAC code\"\n    },\n    \"vesselName\"\
  : {\n      \"type\": \"string\"\n    },\n    \"voyageNumber\": {\n      \"type\": \"string\"\n    },\n    \"currentStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\"Empty\", \"Loaded\", \"OnVessel\", \"AtPort\", \"InTransit\", \"Delivered\"]\n    },\n    \"originPort\": {\n      \"$ref\": \"#/$defs/Port\"\n    },\n    \"destinationPort\": {\n      \"$ref\": \"#/$defs/Port\"\n    },\n    \"estimatedArrival\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Estimated arrival at destination port\"\n    },\n    \"actualArrival\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Actual arrival at destination port\"\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"description\": \"Chronological list of tracking events\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TrackingEvent\"\n      }\n    },\n    \"lastUpdated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  \n    }\n  },\n  \"$defs\": {\n    \"Port\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"locode\": {\n          \"type\": \"string\",\n          \"description\": \"UN/LOCODE (e.g., USNYC, CNSHA)\",\n          \"pattern\": \"^[A-Z]{5}$\"\n        },\n        \"portName\": {\n          \"type\": \"string\"\n        },\n        \"countryCode\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{2}$\"\n        },\n        \"terminalName\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"TrackingEvent\": {\n      \"type\": \"object\",\n      \"required\": [\"eventType\", \"eventTime\"],\n      \"properties\": {\n        \"eventId\": {\n          \"type\": \"string\"\n        },\n        \"eventType\": {\n          \"type\": \"string\",\n          \"enum\": [\"GateIn\", \"GateOut\", \"Load\", \"Discharge\", \"Departure\", \"Arrival\", \"Customs\", \"Delivery\", \"EmptyReturn\"]\n        },\n        \"description\": {\n          \"\
  type\": \"string\"\n        },\n        \"location\": {\n          \"$ref\": \"#/$defs/Port\"\n        },\n        \"vesselName\": {\n          \"type\": \"string\"\n        },\n        \"voyageNumber\": {\n          \"type\": \"string\"\n        },\n        \"eventTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"isActual\": {\n          \"type\": \"boolean\",\n          \"description\": \"true = actual event, false = estimated event\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cargosmart/refs/heads/main/json-schema/cargosmart-container-schema.json
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
title: CargoSmart Container Tracking
---
