---
description: A container or cargo unit managed within the Navis N4 Terminal Operating System
layout: schema
name: Navis N4 Container Unit
properties_list:
- description: ISO 6346 container number
  name: unitNbr
  type: string
- description: N4 internal unit identifier
  name: unitId
  type: integer
- description: Container category in terminal operations
  name: category
  type: string
- description: Full Container Load, Less Container Load, or Empty
  name: freightKind
  type: string
- description: Equipment type code (CTR, TRL, etc.)
  name: equipmentType
  type: string
- description: Container length in feet
  name: equipmentLength
  type: integer
- description: Shipping line SCAC code
  name: lineOperator
  type: string
- description: ''
  name: currentPosition
  type: object
- description: Visit ID of the vessel that delivered the container
  name: arrivalVesselVisit
  type:
  - string
  - 'null'
- description: Visit ID of the vessel that will take the container
  name: departureVesselVisit
  type:
  - string
  - 'null'
- description: ''
  name: holds
  type: array
- description: ''
  name: hazardous
  type: boolean
- description: IMDG dangerous goods class (e.g., 3.0 for flammable liquids)
  name: imdgClass
  type:
  - string
  - 'null'
- description: Whether the container requires temperature control
  name: reefer
  type: boolean
- description: Required setpoint temperature in Celsius for reefer units
  name: temperature
  type:
  - number
  - 'null'
- description: Gross weight in kilograms
  name: weight
  type:
  - number
  - 'null'
- description: Timestamp when the unit entered the terminal
  name: inGateDate
  type:
  - string
  - 'null'
- description: Timestamp when the unit departed the terminal
  name: outGateDate
  type:
  - string
  - 'null'
provider_name: Navis (Kaleris)
provider_slug: navis
schema_file: json-schema/navis-unit-schema.json
slug: navis-unit
source_filename: navis-unit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/navis/refs/heads/main/json-schema/navis-unit-schema.json\",\n  \"title\": \"Navis N4 Container Unit\",\n  \"description\": \"A container or cargo unit managed within the Navis N4 Terminal Operating System\",\n  \"type\": \"object\",\n  \"required\": [\"unitNbr\", \"category\", \"freightKind\"],\n  \"properties\": {\n    \"unitNbr\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 6346 container number\",\n      \"pattern\": \"^[A-Z]{4}[0-9]{7}$\"\n    },\n    \"unitId\": {\n      \"type\": \"integer\",\n      \"description\": \"N4 internal unit identifier\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"enum\": [\"IMPORT\", \"EXPORT\", \"TRANSSHIP\", \"EMPTY\"],\n      \"description\": \"Container category in terminal operations\"\n    },\n    \"freightKind\": {\n      \"type\": \"string\",\n      \"enum\": [\"FCL\"\
  , \"LCL\", \"MTY\"],\n      \"description\": \"Full Container Load, Less Container Load, or Empty\"\n    },\n    \"equipmentType\": {\n      \"type\": \"string\",\n      \"description\": \"Equipment type code (CTR, TRL, etc.)\"\n    },\n    \"equipmentLength\": {\n      \"type\": \"integer\",\n      \"enum\": [20, 40, 45, 48, 53],\n      \"description\": \"Container length in feet\"\n    },\n    \"lineOperator\": {\n      \"type\": \"string\",\n      \"description\": \"Shipping line SCAC code\"\n    },\n    \"currentPosition\": {\n      \"$ref\": \"#/$defs/YardPosition\"\n    },\n    \"arrivalVesselVisit\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Visit ID of the vessel that delivered the container\"\n    },\n    \"departureVesselVisit\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Visit ID of the vessel that will take the container\"\n    },\n    \"holds\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/Hold\"\
  \ }\n    },\n    \"hazardous\": {\n      \"type\": \"boolean\"\n    },\n    \"imdgClass\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"IMDG dangerous goods class (e.g., 3.0 for flammable liquids)\"\n    },\n    \"reefer\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the container requires temperature control\"\n    },\n    \"temperature\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Required setpoint temperature in Celsius for reefer units\"\n    },\n    \"weight\": {\n      \"type\": [\"number\", \"null\"],\n      \"minimum\": 0,\n      \"description\": \"Gross weight in kilograms\"\n    },\n    \"inGateDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the unit entered the terminal\"\n    },\n    \"outGateDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the unit departed\
  \ the terminal\"\n    }\n  },\n  \"$defs\": {\n    \"YardPosition\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"locType\": {\n          \"type\": \"string\",\n          \"enum\": [\"YARD\", \"VESSEL\", \"TRUCK\", \"RAIL\", \"DOCK\", \"VESSEL_BUFFER\"]\n        },\n        \"blockName\": { \"type\": \"string\" },\n        \"bayNbr\": { \"type\": \"integer\" },\n        \"rowNbr\": { \"type\": \"integer\" },\n        \"tierNbr\": { \"type\": \"integer\" },\n        \"slotName\": {\n          \"type\": \"string\",\n          \"description\": \"Full slot identifier (block-bay-row-tier)\"\n        }\n      }\n    },\n    \"Hold\": {\n      \"type\": \"object\",\n      \"required\": [\"holdType\", \"holdStatus\"],\n      \"properties\": {\n        \"holdId\": { \"type\": \"string\" },\n        \"holdType\": {\n          \"type\": \"string\",\n          \"description\": \"Hold type code (CUSTOMS, LINE, PORT, FREIGHT)\"\n        },\n        \"holdStatus\": {\n         \
  \ \"type\": \"string\",\n          \"enum\": [\"ACTIVE\", \"RELEASED\", \"EXPIRED\"]\n        },\n        \"appliedBy\": { \"type\": \"string\" },\n        \"appliedDate\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"releasedDate\": { \"type\": [\"string\", \"null\"], \"format\": \"date-time\" },\n        \"reason\": { \"type\": \"string\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navis/refs/heads/main/json-schema/navis-unit-schema.json
tags:
- Maritime
- Port
- Terminal
- Container
- Logistics
title: Navis N4 Container Unit
---
