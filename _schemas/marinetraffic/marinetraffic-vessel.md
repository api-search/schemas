---
description: AIS vessel position and static data record from MarineTraffic
layout: schema
name: MarineTraffic Vessel
properties_list:
- description: Maritime Mobile Service Identity (9 digits)
  name: MMSI
  type: string
- description: IMO number (7 digits)
  name: IMO
  type:
  - integer
  - 'null'
- description: MarineTraffic internal vessel identifier
  name: SHIP_ID
  type: integer
- description: Latitude in decimal degrees (WGS84)
  name: LAT
  type: number
- description: Longitude in decimal degrees (WGS84)
  name: LON
  type: number
- description: Speed over ground in tenths of knots
  name: SPEED
  type: number
- description: True heading 0-359; 511 = not available
  name: HEADING
  type: integer
- description: Course over ground in tenths of degrees
  name: COURSE
  type: number
- description: AIS navigational status (0=Under way using engine, 1=At anchor, etc.)
  name: STATUS
  type: integer
- description: UTC timestamp of the AIS position report
  name: TIMESTAMP
  type: string
- description: 'Data source: TER = terrestrial AIS, SAT = satellite AIS'
  name: DSRC
  type: string
- description: ''
  name: VESSEL_NAME
  type: string
- description: ''
  name: CALLSIGN
  type: string
- description: Flag state country code (ISO 3166-1 alpha-2)
  name: FLAG
  type: string
- description: AIS vessel type code per ITU-R M.1371
  name: SHIPTYPE
  type: integer
- description: Cargo type code from AIS message type 5
  name: CARGO
  type: integer
- description: ''
  name: CURRENT_PORT
  type: string
- description: ''
  name: LAST_PORT
  type: string
- description: ''
  name: NEXT_PORT_NAME
  type: string
- description: UN/LOCODE of the destination port
  name: NEXT_PORT_UNLOCODE
  type: string
- description: Estimated time of arrival at destination
  name: ETA
  type:
  - string
  - 'null'
- description: Voyage destination as broadcast in AIS
  name: DESTINATION
  type: string
- description: Length overall in meters
  name: LENGTH
  type: integer
- description: Beam/width in meters
  name: WIDTH
  type: integer
- description: Current static draught in tenths of meters
  name: DRAUGHT
  type: number
- description: Gross tonnage
  name: GT
  type: integer
- description: Deadweight tonnage
  name: DWT
  type: integer
- description: ''
  name: YEAR_BUILT
  type:
  - integer
  - 'null'
provider_name: MarineTraffic
provider_slug: marinetraffic
schema_file: json-schema/marinetraffic-vessel-schema.json
slug: marinetraffic-vessel
source_filename: marinetraffic-vessel-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/marinetraffic/refs/heads/main/json-schema/marinetraffic-vessel-schema.json\",\n  \"title\": \"MarineTraffic Vessel\",\n  \"description\": \"AIS vessel position and static data record from MarineTraffic\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MMSI\": {\n      \"type\": \"string\",\n      \"description\": \"Maritime Mobile Service Identity (9 digits)\",\n      \"pattern\": \"^[0-9]{9}$\"\n    },\n    \"IMO\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"IMO number (7 digits)\"\n    },\n    \"SHIP_ID\": {\n      \"type\": \"integer\",\n      \"description\": \"MarineTraffic internal vessel identifier\"\n    },\n    \"LAT\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"minimum\": -90,\n      \"maximum\": 90,\n      \"description\": \"Latitude in decimal degrees (WGS84)\"\n    },\n  \
  \  \"LON\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"minimum\": -180,\n      \"maximum\": 180,\n      \"description\": \"Longitude in decimal degrees (WGS84)\"\n    },\n    \"SPEED\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Speed over ground in tenths of knots\"\n    },\n    \"HEADING\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 511,\n      \"description\": \"True heading 0-359; 511 = not available\"\n    },\n    \"COURSE\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 360,\n      \"description\": \"Course over ground in tenths of degrees\"\n    },\n    \"STATUS\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 15,\n      \"description\": \"AIS navigational status (0=Under way using engine, 1=At anchor, etc.)\"\n    },\n    \"TIMESTAMP\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"\
  UTC timestamp of the AIS position report\"\n    },\n    \"DSRC\": {\n      \"type\": \"string\",\n      \"enum\": [\"TER\", \"SAT\"],\n      \"description\": \"Data source: TER = terrestrial AIS, SAT = satellite AIS\"\n    },\n    \"VESSEL_NAME\": {\n      \"type\": \"string\",\n      \"maxLength\": 20\n    },\n    \"CALLSIGN\": {\n      \"type\": \"string\",\n      \"maxLength\": 7\n    },\n    \"FLAG\": {\n      \"type\": \"string\",\n      \"description\": \"Flag state country code (ISO 3166-1 alpha-2)\"\n    },\n    \"SHIPTYPE\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 99,\n      \"description\": \"AIS vessel type code per ITU-R M.1371\"\n    },\n    \"CARGO\": {\n      \"type\": \"integer\",\n      \"description\": \"Cargo type code from AIS message type 5\"\n    },\n    \"CURRENT_PORT\": {\n      \"type\": \"string\"\n    },\n    \"LAST_PORT\": {\n      \"type\": \"string\"\n    },\n    \"NEXT_PORT_NAME\": {\n      \"type\": \"string\"\n    },\n\
  \    \"NEXT_PORT_UNLOCODE\": {\n      \"type\": \"string\",\n      \"description\": \"UN/LOCODE of the destination port\"\n    },\n    \"ETA\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Estimated time of arrival at destination\"\n    },\n    \"DESTINATION\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"Voyage destination as broadcast in AIS\"\n    },\n    \"LENGTH\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Length overall in meters\"\n    },\n    \"WIDTH\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Beam/width in meters\"\n    },\n    \"DRAUGHT\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Current static draught in tenths of meters\"\n    },\n    \"GT\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Gross tonnage\"\n    },\n    \"DWT\": {\n\
  \      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Deadweight tonnage\"\n    },\n    \"YEAR_BUILT\": {\n      \"type\": [\"integer\", \"null\"],\n      \"minimum\": 1800,\n      \"maximum\": 2100\n    }\n  },\n  \"required\": [\"MMSI\", \"LAT\", \"LON\", \"TIMESTAMP\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/marinetraffic/refs/heads/main/json-schema/marinetraffic-vessel-schema.json
tags:
- AIS
- Maritime
- Shipping
- Vessel Tracking
title: MarineTraffic Vessel
---
