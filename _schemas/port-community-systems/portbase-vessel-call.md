---
description: Schema for a vessel call notification in the Portbase Port Community System, representing a vessel's arrival at a Dutch port.
layout: schema
name: Portbase Vessel Call
properties_list:
- description: Portbase system-generated vessel call identifier
  name: vesselCallId
  type: string
- description: IMO vessel identification number (7 digits)
  name: imoNumber
  type: string
- description: Maritime Mobile Service Identity (9 digits)
  name: mmsi
  type: string
- description: Official vessel name
  name: vesselName
  type: string
- description: Radio call sign
  name: callSign
  type: string
- description: ISO 3166-1 alpha-3 flag state code
  name: flag
  type: string
- description: UN/LOCODE of the destination port (e.g., NLRTM)
  name: portCode
  type: string
- description: Terminal code within the port
  name: terminalCode
  type: string
- description: Current vessel call status
  name: status
  type: string
- description: Estimated time of arrival (UTC)
  name: eta
  type: string
- description: Estimated time of departure (UTC)
  name: etd
  type: string
- description: Actual time of arrival (UTC)
  name: ata
  type:
  - string
  - 'null'
- description: Actual time of departure (UTC)
  name: atd
  type:
  - string
  - 'null'
- description: Shipping agent company name or EORI number
  name: shippingAgent
  type: string
- description: Whether pilotage is required for this vessel call
  name: pilotageRequired
  type: boolean
- description: Whether tug assistance has been requested
  name: tugAssistance
  type: boolean
- description: Maximum forward draft in meters
  name: maxDraftForward
  type: number
- description: Maximum aft draft in meters
  name: maxDraftAft
  type: number
- description: Gross tonnage of the vessel
  name: grossTonnage
  type: integer
- description: Net tonnage of the vessel
  name: netTonnage
  type: integer
provider_name: Port Community Systems
provider_slug: port-community-systems
schema_file: json-schema/portbase-vessel-call-schema.json
slug: portbase-vessel-call
source_filename: portbase-vessel-call-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/port-community-systems/json-schema/portbase-vessel-call-schema.json\",\n  \"title\": \"Portbase Vessel Call\",\n  \"description\": \"Schema for a vessel call notification in the Portbase Port Community System, representing a vessel's arrival at a Dutch port.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vesselCallId\": {\n      \"type\": \"string\",\n      \"description\": \"Portbase system-generated vessel call identifier\"\n    },\n    \"imoNumber\": {\n      \"type\": \"string\",\n      \"pattern\": \"^\\\\d{7}$\",\n      \"description\": \"IMO vessel identification number (7 digits)\"\n    },\n    \"mmsi\": {\n      \"type\": \"string\",\n      \"pattern\": \"^\\\\d{9}$\",\n      \"description\": \"Maritime Mobile Service Identity (9 digits)\"\n    },\n    \"vesselName\": {\n      \"type\": \"string\",\n      \"description\": \"Official vessel name\"\
  \n    },\n    \"callSign\": {\n      \"type\": \"string\",\n      \"description\": \"Radio call sign\"\n    },\n    \"flag\": {\n      \"type\": \"string\",\n      \"maxLength\": 3,\n      \"description\": \"ISO 3166-1 alpha-3 flag state code\"\n    },\n    \"portCode\": {\n      \"type\": \"string\",\n      \"description\": \"UN/LOCODE of the destination port (e.g., NLRTM)\"\n    },\n    \"terminalCode\": {\n      \"type\": \"string\",\n      \"description\": \"Terminal code within the port\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"EXPECTED\", \"ARRIVED\", \"BERTHED\", \"DEPARTED\", \"CANCELLED\"],\n      \"description\": \"Current vessel call status\"\n    },\n    \"eta\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Estimated time of arrival (UTC)\"\n    },\n    \"etd\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Estimated time of departure (UTC)\"\n    },\n\
  \    \"ata\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Actual time of arrival (UTC)\"\n    },\n    \"atd\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Actual time of departure (UTC)\"\n    },\n    \"shippingAgent\": {\n      \"type\": \"string\",\n      \"description\": \"Shipping agent company name or EORI number\"\n    },\n    \"pilotageRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether pilotage is required for this vessel call\"\n    },\n    \"tugAssistance\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether tug assistance has been requested\"\n    },\n    \"maxDraftForward\": {\n      \"type\": \"number\",\n      \"description\": \"Maximum forward draft in meters\"\n    },\n    \"maxDraftAft\": {\n      \"type\": \"number\",\n      \"description\": \"Maximum aft draft in meters\"\n    },\n    \"grossTonnage\": {\n    \
  \  \"type\": \"integer\",\n      \"description\": \"Gross tonnage of the vessel\"\n    },\n    \"netTonnage\": {\n      \"type\": \"integer\",\n      \"description\": \"Net tonnage of the vessel\"\n    }\n  },\n  \"required\": [\"imoNumber\", \"vesselName\", \"portCode\", \"eta\", \"etd\", \"status\"],\n  \"examples\": [\n    {\n      \"vesselCallId\": \"RTM-2026-00987654\",\n      \"imoNumber\": \"9811614\",\n      \"mmsi\": \"636020485\",\n      \"vesselName\": \"MSC OSCAR\",\n      \"callSign\": \"A8IG5\",\n      \"flag\": \"LBR\",\n      \"portCode\": \"NLRTM\",\n      \"terminalCode\": \"ECT-DELTA\",\n      \"status\": \"EXPECTED\",\n      \"eta\": \"2026-03-22T06:00:00Z\",\n      \"etd\": \"2026-03-24T18:00:00Z\",\n      \"ata\": null,\n      \"atd\": null,\n      \"shippingAgent\": \"MSC AGENCY ROTTERDAM\",\n      \"pilotageRequired\": true,\n      \"tugAssistance\": true,\n      \"grossTonnage\": 197362\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/port-community-systems/refs/heads/main/json-schema/portbase-vessel-call-schema.json
tags:
- Maritime
- Port
- Logistics
- Customs
- Cargo
- Shipping
title: Portbase Vessel Call
---
