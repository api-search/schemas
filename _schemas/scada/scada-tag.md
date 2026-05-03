---
description: Schema for a SCADA data tag representing a sensor reading, setpoint, or control variable
layout: schema
name: ScadaTag
properties_list:
- description: Unique identifier for the tag in the SCADA system
  name: tagId
  type: string
- description: Human-readable name for the tag
  name: tagName
  type: string
- description: Hierarchical path to the tag in the SCADA tag browser
  name: tagPath
  type: string
- description: Current value of the tag (type depends on dataType)
  name: value
  type: object
- description: Data type of the tag value
  name: dataType
  type: string
- description: ISO 8601 timestamp of the tag reading
  name: timestamp
  type: string
- description: OPC-UA quality code indicating data reliability
  name: quality
  type: string
- description: Physical engineering units for the tag value
  name: engineeringUnits
  type: string
- description: Human-readable description of what the tag measures
  name: description
  type: string
- description: Configured alarm threshold limits for the tag
  name: alarmLimits
  type: object
- description: Source field device information
  name: deviceSource
  type: object
- description: Logical process area or plant unit this tag belongs to
  name: processArea
  type: string
provider_name: SCADA
provider_slug: scada
schema_file: json-schema/scada-tag-schema.json
slug: scada-tag
source_filename: scada-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/scada/main/json-schema/scada-tag-schema.json\",\n  \"title\": \"ScadaTag\",\n  \"description\": \"Schema for a SCADA data tag representing a sensor reading, setpoint, or control variable\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tagId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the tag in the SCADA system\",\n      \"example\": \"PLANT1.AREA2.PV_101\"\n    },\n    \"tagName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the tag\",\n      \"example\": \"Reactor Inlet Pressure\"\n    },\n    \"tagPath\": {\n      \"type\": \"string\",\n      \"description\": \"Hierarchical path to the tag in the SCADA tag browser\",\n      \"example\": \"Plant/Area2/Reactor/PV_101\"\n    },\n    \"value\": {\n      \"description\": \"Current value of the tag (type depends on dataType)\"\
  ,\n      \"example\": 14.7\n    },\n    \"dataType\": {\n      \"type\": \"string\",\n      \"description\": \"Data type of the tag value\",\n      \"enum\": [\"Float\", \"Double\", \"Integer\", \"Boolean\", \"String\", \"DateTime\"],\n      \"example\": \"Float\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the tag reading\",\n      \"example\": \"2026-05-02T14:30:00.000Z\"\n    },\n    \"quality\": {\n      \"type\": \"string\",\n      \"description\": \"OPC-UA quality code indicating data reliability\",\n      \"enum\": [\"Good\", \"Uncertain\", \"Bad\", \"Stale\"],\n      \"example\": \"Good\"\n    },\n    \"engineeringUnits\": {\n      \"type\": \"string\",\n      \"description\": \"Physical engineering units for the tag value\",\n      \"example\": \"PSI\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of what the tag measures\"\
  ,\n      \"example\": \"Pressure at reactor inlet measured by differential pressure transmitter PV-101\"\n    },\n    \"alarmLimits\": {\n      \"type\": \"object\",\n      \"description\": \"Configured alarm threshold limits for the tag\",\n      \"properties\": {\n        \"highHigh\": {\n          \"type\": \"number\",\n          \"description\": \"High-High alarm setpoint (critical)\"\n        },\n        \"high\": {\n          \"type\": \"number\",\n          \"description\": \"High alarm setpoint (warning)\"\n        },\n        \"low\": {\n          \"type\": \"number\",\n          \"description\": \"Low alarm setpoint (warning)\"\n        },\n        \"lowLow\": {\n          \"type\": \"number\",\n          \"description\": \"Low-Low alarm setpoint (critical)\"\n        }\n      }\n    },\n    \"deviceSource\": {\n      \"type\": \"object\",\n      \"description\": \"Source field device information\",\n      \"properties\": {\n        \"deviceId\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Identifier of the PLC or RTU providing the tag\"\n        },\n        \"deviceType\": {\n          \"type\": \"string\",\n          \"description\": \"Type of source device\",\n          \"enum\": [\"PLC\", \"RTU\", \"DCS\", \"IED\", \"Sensor\", \"Controller\"]\n        },\n        \"protocol\": {\n          \"type\": \"string\",\n          \"description\": \"Communication protocol used to read this tag\",\n          \"enum\": [\"Modbus-TCP\", \"OPC-UA\", \"DNP3\", \"EtherNet/IP\", \"PROFINET\", \"BACnet\", \"MQTT\"]\n        }\n      }\n    },\n    \"processArea\": {\n      \"type\": \"string\",\n      \"description\": \"Logical process area or plant unit this tag belongs to\",\n      \"example\": \"Reactor Section\"\n    }\n  },\n  \"required\": [\"tagId\", \"value\", \"dataType\", \"timestamp\", \"quality\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scada/refs/heads/main/json-schema/scada-tag-schema.json
tags:
- Critical Infrastructure
- ICS
- Industrial Automation
- Industrial IoT
- OT Security
- SCADA
title: ScadaTag
---
