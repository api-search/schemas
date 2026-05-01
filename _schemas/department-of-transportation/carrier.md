---
description: A motor carrier registered with the Federal Motor Carrier Safety Administration.
layout: schema
name: Motor Carrier (FMCSA)
properties_list:
- description: ''
  name: dotNumber
  type: integer
- description: ''
  name: legalName
  type: string
- description: ''
  name: dbaName
  type:
  - string
  - 'null'
- description: ''
  name: ein
  type: string
- description: ''
  name: allowedToOperate
  type: string
- description: ''
  name: phyStreet
  type: string
- description: ''
  name: phyCity
  type: string
- description: ''
  name: phyState
  type: string
- description: ''
  name: phyZipcode
  type: string
- description: ''
  name: telephone
  type: string
- description: ''
  name: totalDrivers
  type: integer
- description: ''
  name: totalPowerUnits
  type: integer
- description: ''
  name: statusCode
  type: string
- description: ''
  name: mcs150Date
  type: string
provider_name: Department of Transportation
provider_slug: department-of-transportation
schema_file: json-schema/carrier-schema.json
slug: carrier
source_filename: carrier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/department-of-transportation/schemas/carrier.json\",\n  \"title\": \"Motor Carrier (FMCSA)\",\n  \"description\": \"A motor carrier registered with the Federal Motor Carrier Safety Administration.\",\n  \"type\": \"object\",\n  \"required\": [\"dotNumber\", \"legalName\"],\n  \"properties\": {\n    \"dotNumber\": { \"type\": \"integer\" },\n    \"legalName\": { \"type\": \"string\" },\n    \"dbaName\": { \"type\": [\"string\", \"null\"] },\n    \"ein\": { \"type\": \"string\" },\n    \"allowedToOperate\": { \"type\": \"string\", \"enum\": [\"Y\", \"N\"] },\n    \"phyStreet\": { \"type\": \"string\" },\n    \"phyCity\": { \"type\": \"string\" },\n    \"phyState\": { \"type\": \"string\", \"pattern\": \"^[A-Z]{2}$\" },\n    \"phyZipcode\": { \"type\": \"string\" },\n    \"telephone\": { \"type\": \"string\" },\n    \"totalDrivers\": { \"type\": \"integer\", \"minimum\"\
  : 0 },\n    \"totalPowerUnits\": { \"type\": \"integer\", \"minimum\": 0 },\n    \"statusCode\": { \"type\": \"string\" },\n    \"mcs150Date\": { \"type\": \"string\", \"format\": \"date\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/json-schema/carrier-schema.json
tags:
- Federal Government
- Transportation
- Vehicles
- Aviation
- Motor Carriers
title: Motor Carrier (FMCSA)
---
