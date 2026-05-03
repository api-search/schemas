---
description: Schema for a Samsara fleet vehicle entity as returned by the Samsara REST API. Represents a motorized vehicle tracked in the Samsara platform including cars, trucks, buses, and construction equipment.
layout: schema
name: Samsara Vehicle
properties_list:
- description: Unique Samsara-assigned identifier for the vehicle.
  name: id
  type: string
- description: Human-readable name of the vehicle.
  name: name
  type: string
- description: Vehicle Identification Number (VIN).
  name: vin
  type: string
- description: Customer-defined key-value pairs for external system identifiers.
  name: externalIds
  type: object
- description: Vehicle manufacturer (e.g., Ford, Kenworth, Freightliner).
  name: make
  type: string
- description: Vehicle model name.
  name: model
  type: string
- description: Model year of the vehicle.
  name: year
  type: integer
- description: Vehicle license plate number.
  name: licensePlate
  type: string
- description: Freeform text notes about the vehicle.
  name: notes
  type: string
- description: Tags assigned to this vehicle for organizational grouping.
  name: tags
  type: array
- description: ELD (Electronic Logging Device) configuration for this vehicle.
  name: eldSettings
  type: object
- description: Current engine hours reading.
  name: engineHours
  type: number
- description: Current odometer reading in meters.
  name: odometerMeters
  type: integer
- description: Statically assigned driver for this vehicle (optional).
  name: staticAssignedDriver
  type: object
provider_name: Samsara
provider_slug: samsara
schema_file: json-schema/samsara-vehicle-schema.json
slug: samsara-vehicle
source_filename: samsara-vehicle-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"samsara-vehicle-schema.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Samsara Vehicle\",\n  \"description\": \"Schema for a Samsara fleet vehicle entity as returned by the Samsara REST API. Represents a motorized vehicle tracked in the Samsara platform including cars, trucks, buses, and construction equipment.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Samsara-assigned identifier for the vehicle.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the vehicle.\"\n    },\n    \"vin\": {\n      \"type\": \"string\",\n      \"description\": \"Vehicle Identification Number (VIN).\",\n      \"pattern\": \"^[A-HJ-NPR-Z0-9]{17}$\"\n    },\n    \"externalIds\": {\n      \"type\": \"object\",\n      \"description\": \"Customer-defined key-value pairs for\
  \ external system identifiers.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"make\": {\n      \"type\": \"string\",\n      \"description\": \"Vehicle manufacturer (e.g., Ford, Kenworth, Freightliner).\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Vehicle model name.\"\n    },\n    \"year\": {\n      \"type\": \"integer\",\n      \"description\": \"Model year of the vehicle.\",\n      \"minimum\": 1900,\n      \"maximum\": 2100\n    },\n    \"licensePlate\": {\n      \"type\": \"string\",\n      \"description\": \"Vehicle license plate number.\"\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Freeform text notes about the vehicle.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags assigned to this vehicle for organizational grouping.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n  \
  \          \"type\": \"string\",\n            \"description\": \"Tag ID.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Tag name.\"\n          },\n          \"parentTagId\": {\n            \"type\": \"string\",\n            \"description\": \"ID of the parent tag in hierarchy.\"\n          }\n        }\n      }\n    },\n    \"eldSettings\": {\n      \"type\": \"object\",\n      \"description\": \"ELD (Electronic Logging Device) configuration for this vehicle.\",\n      \"properties\": {\n        \"eldExempt\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this vehicle is exempt from ELD requirements.\"\n        },\n        \"eldExemptReason\": {\n          \"type\": \"string\",\n          \"description\": \"Reason for ELD exemption if applicable.\"\n        }\n      }\n    },\n    \"engineHours\": {\n      \"type\": \"number\",\n      \"description\": \"Current engine hours reading.\",\n      \"minimum\"\
  : 0\n    },\n    \"odometerMeters\": {\n      \"type\": \"integer\",\n      \"description\": \"Current odometer reading in meters.\",\n      \"minimum\": 0\n    },\n    \"staticAssignedDriver\": {\n      \"type\": \"object\",\n      \"description\": \"Statically assigned driver for this vehicle (optional).\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Driver ID.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Driver name.\"\n        }\n      }\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/samsara/refs/heads/main/json-schema/samsara-vehicle-schema.json
tags:
- Asset Tracking
- Connected Operations
- ELD
- Fleet Management
- GPS Tracking
- IoT
- Logistics
- Safety
- Telematics
- Transportation
title: Samsara Vehicle
---
