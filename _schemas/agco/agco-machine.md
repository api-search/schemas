---
description: An AGCO agricultural machine with telematics capabilities.
layout: schema
name: Machine
properties_list:
- description: Unique machine identifier.
  name: id
  type: string
- description: Machine serial number.
  name: serial_number
  type: string
- description: Machine model name.
  name: model
  type: string
- description: AGCO brand.
  name: brand
  type: string
- description: Machine type.
  name: type
  type: string
- description: Machine connectivity status.
  name: status
  type: string
- description: ''
  name: location
  type: object
- description: Total engine hours.
  name: engine_hours
  type: number
- description: Current fuel level percentage.
  name: fuel_level
  type: number
- description: Record creation timestamp.
  name: created_at
  type: string
- description: Record last updated timestamp.
  name: updated_at
  type: string
provider_name: agco
provider_slug: agco
schema_file: json-schema/agco-machine-schema.json
slug: agco-machine
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agco/refs/heads/main/json-schema/agco-machine-schema.json\",\n  \"title\": \"Machine\",\n  \"description\": \"An AGCO agricultural machine with telematics capabilities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique machine identifier.\",\n      \"example\": \"mach-500123\"\n    },\n    \"serial_number\": {\n      \"type\": \"string\",\n      \"description\": \"Machine serial number.\",\n      \"example\": \"AGC-2025-001234\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Machine model name.\",\n      \"example\": \"Fendt 942 Vario\"\n    },\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"AGCO brand.\",\n      \"enum\": [\n        \"Fendt\",\n        \"Massey Ferguson\",\n        \"Challenger\",\n        \"Valtra\"\
  ,\n        \"GSI\"\n      ],\n      \"example\": \"Fendt\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Machine type.\",\n      \"enum\": [\n        \"tractor\",\n        \"combine\",\n        \"sprayer\",\n        \"planter\",\n        \"harvester\",\n        \"other\"\n      ],\n      \"example\": \"tractor\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Machine connectivity status.\",\n      \"enum\": [\n        \"online\",\n        \"offline\",\n        \"unknown\"\n      ],\n      \"example\": \"online\"\n    },\n    \"location\": {\n      \"$ref\": \"#/definitions/Location\"\n    },\n    \"engine_hours\": {\n      \"type\": \"number\",\n      \"description\": \"Total engine hours.\",\n      \"example\": 1250.5\n    },\n    \"fuel_level\": {\n      \"type\": \"number\",\n      \"description\": \"Current fuel level percentage.\",\n      \"example\": 78.5\n    },\n    \"created_at\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"Record creation timestamp.\",\n      \"example\": \"2025-01-15T09:00:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record last updated timestamp.\",\n      \"example\": \"2025-04-01T12:00:00Z\"\n    }\n  },\n  \"definitions\": {\n    \"Location\": {\n      \"type\": \"object\",\n      \"description\": \"Geographic location coordinates.\",\n      \"properties\": {\n        \"latitude\": {\n          \"type\": \"number\",\n          \"description\": \"Latitude in decimal degrees.\",\n          \"example\": 41.8781\n        },\n        \"longitude\": {\n          \"type\": \"number\",\n          \"description\": \"Longitude in decimal degrees.\",\n          \"example\": -87.6298\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Location timestamp.\",\n         \
  \ \"example\": \"2025-04-01T10:30:00Z\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agco/refs/heads/main/json-schema/agco-machine-schema.json
tags: []
title: Machine
---
