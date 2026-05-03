---
description: Schema for an OSIsoft PI point (tag), the fundamental data storage unit in the PI System representing a single time-series measurement.
layout: schema
name: OSIsoft PI Point
properties_list:
- description: PI Web API opaque unique identifier
  name: WebId
  type: string
- description: PI point numeric ID on the PI Data Archive
  name: Id
  type: integer
- description: PI tag name
  name: Name
  type: string
- description: Full PI path (\\ServerName\TagName)
  name: Path
  type: string
- description: PI point data type
  name: PointType
  type: string
- description: Unit of measure (e.g., kPa, °C, m3/h)
  name: EngineeringUnits
  type: string
- description: Tag description
  name: Description
  type: string
- description: Short descriptor
  name: Descriptor
  type: string
- description: PI point class (classic, base, etc.)
  name: PointClass
  type: string
- description: Zero value for analog points
  name: Zero
  type: number
- description: Span value for analog points
  name: Span
  type: number
- description: Exception minimum for compression
  name: ExcMin
  type: number
- description: Exception maximum for compression
  name: ExcMax
  type: number
- description: True if values are step-function (digital/integer types)
  name: Step
  type: boolean
- description: True if future-dated values are allowed
  name: Future
  type: boolean
- description: Tag name alias
  name: Tag
  type: string
- description: Instrument tag reference
  name: Instrument
  type: string
- description: Location attribute 1
  name: Location1
  type: integer
- description: Location attribute 2
  name: Location2
  type: integer
- description: Location attribute 3
  name: Location3
  type: integer
- description: Location attribute 4
  name: Location4
  type: integer
- description: Location attribute 5
  name: Location5
  type: integer
provider_name: osisoft-pi
provider_slug: osisoft-pi
schema_file: json-schema/osisoft-pi-point-schema.json
slug: osisoft-pi-point
source_filename: osisoft-pi-point-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/osisoft-pi/json-schema/osisoft-pi-point-schema.json\",\n  \"title\": \"OSIsoft PI Point\",\n  \"description\": \"Schema for an OSIsoft PI point (tag), the fundamental data storage unit in the PI System representing a single time-series measurement.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"WebId\": {\n      \"type\": \"string\",\n      \"description\": \"PI Web API opaque unique identifier\"\n    },\n    \"Id\": {\n      \"type\": \"integer\",\n      \"description\": \"PI point numeric ID on the PI Data Archive\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"maxLength\": 80,\n      \"description\": \"PI tag name\"\n    },\n    \"Path\": {\n      \"type\": \"string\",\n      \"description\": \"Full PI path (\\\\\\\\ServerName\\\\TagName)\"\n    },\n    \"PointType\": {\n      \"type\": \"string\",\n      \"enum\": [\"Float16\", \"\
  Float32\", \"Float64\", \"Int16\", \"Int32\", \"Digital\", \"Timestamp\", \"String\"],\n      \"description\": \"PI point data type\"\n    },\n    \"EngineeringUnits\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measure (e.g., kPa, °C, m3/h)\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"maxLength\": 128,\n      \"description\": \"Tag description\"\n    },\n    \"Descriptor\": {\n      \"type\": \"string\",\n      \"maxLength\": 32,\n      \"description\": \"Short descriptor\"\n    },\n    \"PointClass\": {\n      \"type\": \"string\",\n      \"description\": \"PI point class (classic, base, etc.)\"\n    },\n    \"Zero\": {\n      \"type\": \"number\",\n      \"description\": \"Zero value for analog points\"\n    },\n    \"Span\": {\n      \"type\": \"number\",\n      \"description\": \"Span value for analog points\"\n    },\n    \"ExcMin\": {\n      \"type\": \"number\",\n      \"description\": \"Exception minimum for compression\"\n    },\n\
  \    \"ExcMax\": {\n      \"type\": \"number\",\n      \"description\": \"Exception maximum for compression\"\n    },\n    \"Step\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if values are step-function (digital/integer types)\"\n    },\n    \"Future\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if future-dated values are allowed\"\n    },\n    \"Tag\": {\n      \"type\": \"string\",\n      \"description\": \"Tag name alias\"\n    },\n    \"Instrument\": {\n      \"type\": \"string\",\n      \"description\": \"Instrument tag reference\"\n    },\n    \"Location1\": { \"type\": \"integer\", \"description\": \"Location attribute 1\" },\n    \"Location2\": { \"type\": \"integer\", \"description\": \"Location attribute 2\" },\n    \"Location3\": { \"type\": \"integer\", \"description\": \"Location attribute 3\" },\n    \"Location4\": { \"type\": \"integer\", \"description\": \"Location attribute 4\" },\n    \"Location5\": { \"type\": \"integer\", \"\
  description\": \"Location attribute 5\" }\n  },\n  \"required\": [\"WebId\", \"Name\", \"PointType\"],\n  \"examples\": [\n    {\n      \"WebId\": \"P0UKSmL5GxNku5bXVjXV1zIgAAAUEkT0NPRFwtUEkxXFJFQUNUT1IuVEVNUC5QVjE\",\n      \"Id\": 1042,\n      \"Name\": \"REACTOR.TEMP.PV1\",\n      \"Path\": \"\\\\\\\\PI-SERVER1\\\\REACTOR.TEMP.PV1\",\n      \"PointType\": \"Float32\",\n      \"EngineeringUnits\": \"°C\",\n      \"Description\": \"Reactor 1 Temperature Process Variable\",\n      \"Descriptor\": \"R1 Temp\",\n      \"PointClass\": \"classic\",\n      \"Zero\": -50,\n      \"Span\": 250,\n      \"Step\": false,\n      \"Future\": false\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/osisoft-pi/refs/heads/main/json-schema/osisoft-pi-point-schema.json
tags: []
title: OSIsoft PI Point
---
