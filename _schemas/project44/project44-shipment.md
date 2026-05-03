---
description: Schema for a project44 multimodal freight shipment with tracking and visibility data.
layout: schema
name: project44 Shipment
properties_list:
- description: project44 internal shipment UUID
  name: id
  type: string
- description: Unique master shipment identifier across modes
  name: masterShipmentId
  type: string
- description: Transportation mode
  name: mode
  type: string
- description: Current lifecycle status
  name: status
  type: string
- description: Carrier SCAC code
  name: carrierCode
  type: string
- description: ''
  name: carrierName
  type: string
- description: Carrier PRO/tracking number
  name: proNumber
  type: string
- description: Bill of lading number
  name: bolNumber
  type: string
- description: Purchase order number
  name: poNumber
  type: string
- description: ''
  name: origin
  type: object
- description: ''
  name: destination
  type: object
- description: ''
  name: estimatedDelivery
  type: object
- description: ''
  name: currentPosition
  type: object
- description: ''
  name: exceptions
  type: array
- description: ''
  name: createDatetime
  type: string
- description: ''
  name: lastUpdateDatetime
  type: string
provider_name: project44
provider_slug: project44
schema_file: json-schema/project44-shipment-schema.json
slug: project44-shipment
source_filename: project44-shipment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/project44/json-schema/project44-shipment-schema.json\",\n  \"title\": \"project44 Shipment\",\n  \"description\": \"Schema for a project44 multimodal freight shipment with tracking and visibility data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"project44 internal shipment UUID\"\n    },\n    \"masterShipmentId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique master shipment identifier across modes\"\n    },\n    \"mode\": {\n      \"type\": \"string\",\n      \"enum\": [\"TL\", \"LTL\", \"OCEAN\", \"AIR\", \"RAIL\", \"PARCEL\", \"DRAY\"],\n      \"description\": \"Transportation mode\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"AT_STOP\", \"IN_TRANSIT\", \"COMPLETED\", \"EXCEPTION\", \"UNKNOWN\"],\n      \"\
  description\": \"Current lifecycle status\"\n    },\n    \"carrierCode\": {\n      \"type\": \"string\",\n      \"description\": \"Carrier SCAC code\"\n    },\n    \"carrierName\": {\n      \"type\": \"string\"\n    },\n    \"proNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Carrier PRO/tracking number\"\n    },\n    \"bolNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Bill of lading number\"\n    },\n    \"poNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Purchase order number\"\n    },\n    \"origin\": {\n      \"$ref\": \"#/$defs/ShipmentStop\"\n    },\n    \"destination\": {\n      \"$ref\": \"#/$defs/ShipmentStop\"\n    },\n    \"estimatedDelivery\": {\n      \"$ref\": \"#/$defs/ETAWindow\"\n    },\n    \"currentPosition\": {\n      \"$ref\": \"#/$defs/Position\"\n    },\n    \"exceptions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ShipmentException\"\n      }\n    },\n    \"createDatetime\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"lastUpdateDatetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\"id\", \"mode\", \"status\", \"carrierCode\"],\n  \"$defs\": {\n    \"ShipmentStop\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"stopNumber\": { \"type\": \"integer\" },\n        \"stopType\": { \"type\": \"string\", \"enum\": [\"ORIGIN\", \"DESTINATION\", \"INTERMEDIATE\"] },\n        \"name\": { \"type\": \"string\" },\n        \"city\": { \"type\": \"string\" },\n        \"state\": { \"type\": \"string\" },\n        \"postalCode\": { \"type\": \"string\" },\n        \"country\": { \"type\": \"string\", \"maxLength\": 3 },\n        \"latitude\": { \"type\": \"number\", \"format\": \"double\" },\n        \"longitude\": { \"type\": \"number\", \"format\": \"double\" },\n        \"actualArrival\": { \"type\": [\"string\", \"null\"], \"format\": \"date-time\" },\n    \
  \    \"actualDeparture\": { \"type\": [\"string\", \"null\"], \"format\": \"date-time\" }\n      }\n    },\n    \"ETAWindow\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"estimatedAt\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"confidenceLow\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"confidenceHigh\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"predictedOnTime\": { \"type\": \"boolean\" },\n        \"predictedLateMinutes\": { \"type\": [\"integer\", \"null\"] }\n      }\n    },\n    \"Position\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"timestamp\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"latitude\": { \"type\": \"number\", \"format\": \"double\" },\n        \"longitude\": { \"type\": \"number\", \"format\": \"double\" },\n        \"heading\": { \"type\": [\"number\", \"null\"], \"format\": \"double\" },\n        \"speed\": { \"type\": [\"number\",\
  \ \"null\"], \"format\": \"double\" },\n        \"speedUnit\": { \"type\": \"string\", \"enum\": [\"MPH\", \"KPH\"] }\n      },\n      \"required\": [\"timestamp\", \"latitude\", \"longitude\"]\n    },\n    \"ShipmentException\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"exceptionCode\": { \"type\": \"string\" },\n        \"description\": { \"type\": \"string\" },\n        \"severity\": { \"type\": \"string\", \"enum\": [\"LOW\", \"MEDIUM\", \"HIGH\", \"CRITICAL\"] },\n        \"timestamp\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"resolvedAt\": { \"type\": [\"string\", \"null\"], \"format\": \"date-time\" }\n      }\n    }\n  },\n  \"examples\": [\n    {\n      \"id\": \"f7a3b2c1-1234-5678-abcd-ef0123456789\",\n      \"masterShipmentId\": \"MSI-TL-2026031800001\",\n      \"mode\": \"TL\",\n      \"status\": \"IN_TRANSIT\",\n      \"carrierCode\": \"ODFL\",\n      \"carrierName\": \"Old Dominion Freight Line\",\n      \"proNumber\": \"ODFL-58712346\"\
  ,\n      \"bolNumber\": \"BOL-202603180001\",\n      \"origin\": {\n        \"stopNumber\": 1,\n        \"stopType\": \"ORIGIN\",\n        \"city\": \"Chicago\",\n        \"state\": \"IL\",\n        \"postalCode\": \"60608\",\n        \"country\": \"USA\"\n      },\n      \"destination\": {\n        \"stopNumber\": 2,\n        \"stopType\": \"DESTINATION\",\n        \"city\": \"Atlanta\",\n        \"state\": \"GA\",\n        \"postalCode\": \"30303\",\n        \"country\": \"USA\"\n      },\n      \"estimatedDelivery\": {\n        \"estimatedAt\": \"2026-03-20T14:00:00Z\",\n        \"confidenceLow\": \"2026-03-20T12:00:00Z\",\n        \"confidenceHigh\": \"2026-03-20T17:00:00Z\",\n        \"predictedOnTime\": true\n      }\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/project44/refs/heads/main/json-schema/project44-shipment-schema.json
tags:
- Logistics
- Freight
- Supply Chain
- Visibility
- Tracking
- Transportation
title: project44 Shipment
---
