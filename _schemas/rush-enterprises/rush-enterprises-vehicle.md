---
description: A commercial vehicle sold or serviced by Rush Truck Centers
layout: schema
name: Rush Enterprises Commercial Vehicle
properties_list:
- description: Unique vehicle identifier
  name: vehicleId
  type: string
- description: Vehicle Identification Number (17 characters)
  name: vin
  type: string
- description: Vehicle condition
  name: type
  type: string
- description: Manufacturer (Peterbilt, International, Hino, etc.)
  name: make
  type: string
- description: Vehicle model
  name: model
  type: string
- description: Model year
  name: year
  type: integer
- description: Vehicle category (semi-truck, medium-duty, etc.)
  name: category
  type: string
- description: Odometer reading in miles
  name: mileage
  type: integer
- description: List price in USD
  name: price
  type: number
- description: Rush Truck Center location name
  name: location
  type: string
provider_name: Rush Enterprises
provider_slug: rush-enterprises
schema_file: json-schema/rush-enterprises-vehicle-schema.json
slug: rush-enterprises-vehicle
source_filename: rush-enterprises-vehicle-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://api-evangelist.github.io/rush-enterprises/json-schema/rush-enterprises-vehicle-schema.json\",\n  \"title\": \"Rush Enterprises Commercial Vehicle\",\n  \"description\": \"A commercial vehicle sold or serviced by Rush Truck Centers\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vehicleId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique vehicle identifier\"\n    },\n    \"vin\": {\n      \"type\": \"string\",\n      \"description\": \"Vehicle Identification Number (17 characters)\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"new\", \"used\"],\n      \"description\": \"Vehicle condition\"\n    },\n    \"make\": {\n      \"type\": \"string\",\n      \"description\": \"Manufacturer (Peterbilt, International, Hino, etc.)\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Vehicle model\"\n    },\n    \"year\": {\n\
  \      \"type\": \"integer\",\n      \"description\": \"Model year\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Vehicle category (semi-truck, medium-duty, etc.)\"\n    },\n    \"mileage\": {\n      \"type\": \"integer\",\n      \"description\": \"Odometer reading in miles\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"List price in USD\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Rush Truck Center location name\"\n    }\n  },\n  \"required\": [\"vehicleId\", \"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rush-enterprises/refs/heads/main/json-schema/rush-enterprises-vehicle-schema.json
tags:
- Commercial Vehicles
- Fleet Management
- Telematics
- Truck Dealerships
- Transportation
title: Rush Enterprises Commercial Vehicle
---
