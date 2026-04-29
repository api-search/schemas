---
description: Real-time parking availability data from AppyWay
layout: schema
name: ParkingAvailability
properties_list:
- description: Unique parking location identifier
  name: locationId
  type: string
- description: Parking location name
  name: name
  type: string
- description: Number of available parking spaces
  name: availableSpaces
  type: integer
- description: Total number of parking spaces
  name: totalSpaces
  type: integer
- description: Current occupancy percentage
  name: occupancyPercent
  type: number
- description: Timestamp of availability data
  name: timestamp
  type: string
- description: Geographic coordinates of the parking location
  name: coordinates
  type: object
- description: Whether EV charging is available
  name: evCharging
  type: boolean
- description: Parking restrictions (residents only, time-limited, etc.)
  name: restrictions
  type: array
provider_name: AppyWay
provider_slug: appyway
schema_file: json-schema/parking-availability-schema.json
slug: parking-availability
source_filename: parking-availability-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appyway/main/json-schema/parking-availability-schema.json\",\n  \"title\": \"ParkingAvailability\",\n  \"description\": \"Real-time parking availability data from AppyWay\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"locationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique parking location identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Parking location name\"\n    },\n    \"availableSpaces\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of available parking spaces\"\n    },\n    \"totalSpaces\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of parking spaces\"\n    },\n    \"occupancyPercent\": {\n      \"type\": \"number\",\n      \"description\": \"Current occupancy percentage\"\n    },\n    \"timestamp\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of availability data\"\n    },\n    \"coordinates\": {\n      \"type\": \"object\",\n      \"description\": \"Geographic coordinates of the parking location\",\n      \"properties\": {\n        \"latitude\": {\n          \"type\": \"number\"\n        },\n        \"longitude\": {\n          \"type\": \"number\"\n        }\n      }\n    },\n    \"evCharging\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether EV charging is available\"\n    },\n    \"restrictions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Parking restrictions (residents only, time-limited, etc.)\"\n    }\n  },\n  \"required\": [\n    \"locationId\",\n    \"availableSpaces\",\n    \"totalSpaces\",\n    \"timestamp\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appyway/refs/heads/main/json-schema/parking-availability-schema.json
tags:
- Parking
- Traffic
- Urban Mobility
- Smart Cities
- EV Charging
title: ParkingAvailability
---
