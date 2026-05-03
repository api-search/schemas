---
description: Schema for a Samsara driver safety event as returned by the Samsara Safety API. Represents a detected driving behavior event such as harsh braking, harsh acceleration, harsh cornering, speeding, or camera-detected event.
layout: schema
name: Samsara Safety Event
properties_list:
- description: Unique identifier for the safety event.
  name: id
  type: string
- description: Type of safety event detected.
  name: eventType
  type: string
- description: Timestamp of the safety event in RFC 3339 format.
  name: time
  type: string
- description: The driver involved in the safety event.
  name: driver
  type: object
- description: The vehicle involved in the safety event.
  name: vehicle
  type: object
- description: GPS location where the event occurred.
  name: location
  type: object
- description: Vehicle speed in miles per hour at the time of the event.
  name: speedMilesPerHour
  type: number
- description: Severity level of the safety event.
  name: severity
  type: string
- description: Current coaching workflow state for this event.
  name: coachingState
  type: string
provider_name: Samsara
provider_slug: samsara
schema_file: json-schema/samsara-safety-event-schema.json
slug: samsara-safety-event
source_filename: samsara-safety-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"samsara-safety-event-schema.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Samsara Safety Event\",\n  \"description\": \"Schema for a Samsara driver safety event as returned by the Samsara Safety API. Represents a detected driving behavior event such as harsh braking, harsh acceleration, harsh cornering, speeding, or camera-detected event.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"eventType\", \"time\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the safety event.\"\n    },\n    \"eventType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of safety event detected.\",\n      \"enum\": [\n        \"crashThresholdExceeded\",\n        \"eatingDriving\",\n        \"drowsyDriving\",\n        \"followingDistanceSevere\",\n        \"followingDistanceModerate\",\n        \"handsOffWheel\",\n        \"harshAccel\",\n        \"\
  harshBrake\",\n        \"harshTurn\",\n        \"inattentiveDriving\",\n        \"landDeparture\",\n        \"mobileUsage\",\n        \"obstructedCamera\",\n        \"rollingStopSign\",\n        \"smokingCigarette\",\n        \"speeding\",\n        \"stopSignViolation\",\n        \"tailgating\",\n        \"yawning\"\n      ]\n    },\n    \"time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the safety event in RFC 3339 format.\"\n    },\n    \"driver\": {\n      \"type\": \"object\",\n      \"description\": \"The driver involved in the safety event.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Driver ID.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Driver name.\"\n        }\n      }\n    },\n    \"vehicle\": {\n      \"type\": \"object\",\n      \"description\": \"The vehicle involved in the safety event.\",\n\
  \      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Vehicle ID.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Vehicle name.\"\n        }\n      }\n    },\n    \"location\": {\n      \"type\": \"object\",\n      \"description\": \"GPS location where the event occurred.\",\n      \"properties\": {\n        \"latitude\": {\n          \"type\": \"number\",\n          \"description\": \"Latitude in decimal degrees.\",\n          \"minimum\": -90,\n          \"maximum\": 90\n        },\n        \"longitude\": {\n          \"type\": \"number\",\n          \"description\": \"Longitude in decimal degrees.\",\n          \"minimum\": -180,\n          \"maximum\": 180\n        },\n        \"formattedAddress\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable address of the event location.\"\n        }\n      }\n    },\n    \"speedMilesPerHour\": {\n      \"type\"\
  : \"number\",\n      \"description\": \"Vehicle speed in miles per hour at the time of the event.\",\n      \"minimum\": 0\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"Severity level of the safety event.\",\n      \"enum\": [\"low\", \"medium\", \"high\", \"critical\"]\n    },\n    \"coachingState\": {\n      \"type\": \"string\",\n      \"description\": \"Current coaching workflow state for this event.\",\n      \"enum\": [\"needs_review\", \"dismissed\", \"coached\", \"pending_coach_review\"]\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/samsara/refs/heads/main/json-schema/samsara-safety-event-schema.json
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
title: Samsara Safety Event
---
