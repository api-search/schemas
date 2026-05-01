---
description: A vehicle decoded via the NHTSA vPIC API.
layout: schema
name: Vehicle (NHTSA vPIC)
properties_list:
- description: ''
  name: VIN
  type: string
- description: ''
  name: Make
  type: string
- description: ''
  name: Model
  type: string
- description: ''
  name: ModelYear
  type:
  - string
  - integer
- description: ''
  name: Manufacturer
  type: string
- description: ''
  name: ManufacturerId
  type:
  - string
  - integer
- description: ''
  name: VehicleType
  type: string
- description: ''
  name: BodyClass
  type: string
- description: ''
  name: DriveType
  type: string
- description: ''
  name: EngineCylinders
  type:
  - string
  - integer
- description: ''
  name: EngineHP
  type:
  - string
  - integer
- description: ''
  name: FuelTypePrimary
  type: string
- description: ''
  name: PlantCity
  type: string
- description: ''
  name: PlantState
  type: string
- description: ''
  name: PlantCountry
  type: string
- description: ''
  name: TransmissionStyle
  type: string
- description: ''
  name: Series
  type:
  - string
  - 'null'
- description: ''
  name: Trim
  type:
  - string
  - 'null'
- description: ''
  name: WheelBaseShort
  type:
  - string
  - 'null'
- description: ''
  name: WheelBaseLong
  type:
  - string
  - 'null'
- description: ''
  name: GVWR
  type: string
provider_name: Department of Transportation
provider_slug: department-of-transportation
schema_file: json-schema/vehicle-schema.json
slug: vehicle
source_filename: vehicle-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/department-of-transportation/schemas/vehicle.json\",\n  \"title\": \"Vehicle (NHTSA vPIC)\",\n  \"description\": \"A vehicle decoded via the NHTSA vPIC API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VIN\": { \"type\": \"string\", \"minLength\": 11, \"maxLength\": 17 },\n    \"Make\": { \"type\": \"string\" },\n    \"Model\": { \"type\": \"string\" },\n    \"ModelYear\": { \"type\": [\"string\", \"integer\"] },\n    \"Manufacturer\": { \"type\": \"string\" },\n    \"ManufacturerId\": { \"type\": [\"string\", \"integer\"] },\n    \"VehicleType\": { \"type\": \"string\" },\n    \"BodyClass\": { \"type\": \"string\" },\n    \"DriveType\": { \"type\": \"string\" },\n    \"EngineCylinders\": { \"type\": [\"string\", \"integer\"] },\n    \"EngineHP\": { \"type\": [\"string\", \"integer\"] },\n    \"FuelTypePrimary\": { \"type\": \"string\" },\n    \"PlantCity\"\
  : { \"type\": \"string\" },\n    \"PlantState\": { \"type\": \"string\" },\n    \"PlantCountry\": { \"type\": \"string\" },\n    \"TransmissionStyle\": { \"type\": \"string\" },\n    \"Series\": { \"type\": [\"string\", \"null\"] },\n    \"Trim\": { \"type\": [\"string\", \"null\"] },\n    \"WheelBaseShort\": { \"type\": [\"string\", \"null\"] },\n    \"WheelBaseLong\": { \"type\": [\"string\", \"null\"] },\n    \"GVWR\": { \"type\": \"string\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/json-schema/vehicle-schema.json
tags:
- Federal Government
- Transportation
- Vehicles
- Aviation
- Motor Carriers
title: Vehicle (NHTSA vPIC)
---
