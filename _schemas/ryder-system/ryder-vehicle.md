---
description: A commercial vehicle in the Ryder fleet management system
layout: schema
name: Ryder Vehicle
properties_list:
- description: Unique vehicle identifier
  name: vehicleId
  type: string
- description: Vehicle Identification Number (17 characters)
  name: vin
  type: string
- description: Vehicle manufacturer (e.g., Peterbilt, International, Freightliner)
  name: make
  type: string
- description: Vehicle model
  name: model
  type: string
- description: Model year
  name: year
  type: integer
- description: Current vehicle status
  name: status
  type: string
- description: Current odometer reading in miles
  name: mileage
  type: integer
provider_name: Ryder System
provider_slug: ryder-system
schema_file: json-schema/ryder-vehicle-schema.json
slug: ryder-vehicle
source_filename: ryder-vehicle-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://api-evangelist.github.io/ryder-system/json-schema/ryder-vehicle-schema.json\",\n  \"title\": \"Ryder Vehicle\",\n  \"description\": \"A commercial vehicle in the Ryder fleet management system\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vehicleId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique vehicle identifier\"\n    },\n    \"vin\": {\n      \"type\": \"string\",\n      \"description\": \"Vehicle Identification Number (17 characters)\"\n    },\n    \"make\": {\n      \"type\": \"string\",\n      \"description\": \"Vehicle manufacturer (e.g., Peterbilt, International, Freightliner)\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Vehicle model\"\n    },\n    \"year\": {\n      \"type\": \"integer\",\n      \"description\": \"Model year\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current vehicle\
  \ status\"\n    },\n    \"mileage\": {\n      \"type\": \"integer\",\n      \"description\": \"Current odometer reading in miles\"\n    }\n  },\n  \"required\": [\"vehicleId\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/json-schema/ryder-vehicle-schema.json
tags:
- Fleet Management
- Logistics
- Supply Chain
- Transportation
- Trucking
title: Ryder Vehicle
---
