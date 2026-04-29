---
description: Flight notification message contract
layout: schema
name: FlightNotificationItemContract
properties_list:
- description: Human-readable summary of the flight status update
  name: notificationSummary
  type: string
- description: Human-readable remark to the flight status update
  name: notificationRemark
  type: string
- description: ''
  name: greatCircleDistance
  type: object
- description: ''
  name: departure
  type: object
- description: ''
  name: arrival
  type: object
- description: ''
  name: flightPlan
  type: object
- description: Time (UTC) of the latest update of flight information (excluding Location)
  name: lastUpdatedUtc
  type: string
- description: Flight Number
  name: number
  type: string
- description: ATC call-sign of the flight
  name: callSign
  type: string
- description: ''
  name: status
  type: object
- description: ''
  name: codeshareStatus
  type: object
- description: Is cargo flight
  name: isCargo
  type: boolean
- description: ''
  name: aircraft
  type: object
- description: ''
  name: airline
  type: object
- description: ''
  name: location
  type: object
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-flight-notification-item-contract-schema.json
slug: aerodatabox-flight-notification-item-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-notification-item-contract-schema.json\",\n  \"title\": \"FlightNotificationItemContract\",\n  \"description\": \"Flight notification message contract\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"notificationSummary\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable summary of the flight status update\",\n      \"nullable\": true\n    },\n    \"notificationRemark\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable remark to the flight status update\",\n      \"nullable\": true\n    },\n    \"greatCircleDistance\": {\n      \"$ref\": \"#/components/schemas/Distance\"\n    },\n    \"departure\": {\n      \"$ref\": \"#/components/schemas/FlightAirportMovementContract\"\n    },\n    \"arrival\": {\n      \"$ref\": \"#/components/schemas/FlightAirportMovementContract\"\
  \n    },\n    \"flightPlan\": {\n      \"$ref\": \"#/components/schemas/FlightPlanContract\"\n    },\n    \"lastUpdatedUtc\": {\n      \"type\": \"string\",\n      \"description\": \"Time (UTC) of the latest update of flight information (excluding Location)\",\n      \"format\": \"date-time\"\n    },\n    \"number\": {\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"Flight Number\"\n    },\n    \"callSign\": {\n      \"type\": \"string\",\n      \"description\": \"ATC call-sign of the flight\",\n      \"nullable\": true\n    },\n    \"status\": {\n      \"$ref\": \"#/components/schemas/FlightStatus\"\n    },\n    \"codeshareStatus\": {\n      \"$ref\": \"#/components/schemas/CodeshareStatus\"\n    },\n    \"isCargo\": {\n      \"type\": \"boolean\",\n      \"description\": \"Is cargo flight\"\n    },\n    \"aircraft\": {\n      \"$ref\": \"#/components/schemas/FlightAircraftContract\"\n    },\n    \"airline\": {\n      \"$ref\": \"#/components/schemas/FlightAirlineContract\"\
  \n    },\n    \"location\": {\n      \"$ref\": \"#/components/schemas/FlightLocationContract\"\n    }\n  },\n  \"required\": [\n    \"arrival\",\n    \"codeshareStatus\",\n    \"departure\",\n    \"isCargo\",\n    \"lastUpdatedUtc\",\n    \"number\",\n    \"status\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-notification-item-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: FlightNotificationItemContract
---
