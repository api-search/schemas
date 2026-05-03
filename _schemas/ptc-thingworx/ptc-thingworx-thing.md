---
description: Schema for a PTC ThingWorx thing (digital twin instance), representing a connected industrial asset or device.
layout: schema
name: PTC ThingWorx Thing
properties_list:
- description: Unique thing name in the ThingWorx platform
  name: name
  type: string
- description: Human-readable thing description
  name: description
  type: string
- description: Parent thing template that defines property/service/event shape
  name: thingTemplate
  type: string
- description: Applied thing shape for additional properties or services
  name: thingShape
  type: string
- description: Model tag vocabulary entries for classification
  name: tags
  type: array
- description: Whether the thing is enabled and able to receive data
  name: isEnabled
  type: boolean
- description: True if this is a built-in ThingWorx system object
  name: isSystemObject
  type: boolean
- description: External identifier for mapping to physical device or asset
  name: identifier
  type: string
- description: ThingWorx project the thing belongs to
  name: projectName
  type: string
- description: Last modification timestamp (epoch milliseconds UTC)
  name: lastModifiedDate
  type: integer
provider_name: ptc-thingworx
provider_slug: ptc-thingworx
schema_file: json-schema/ptc-thingworx-thing-schema.json
slug: ptc-thingworx-thing
source_filename: ptc-thingworx-thing-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/ptc-thingworx/json-schema/ptc-thingworx-thing-schema.json\",\n  \"title\": \"PTC ThingWorx Thing\",\n  \"description\": \"Schema for a PTC ThingWorx thing (digital twin instance), representing a connected industrial asset or device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique thing name in the ThingWorx platform\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable thing description\"\n    },\n    \"thingTemplate\": {\n      \"type\": \"string\",\n      \"description\": \"Parent thing template that defines property/service/event shape\"\n    },\n    \"thingShape\": {\n      \"type\": \"string\",\n      \"description\": \"Applied thing shape for additional properties or services\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\
  ,\n      \"description\": \"Model tag vocabulary entries for classification\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": { \"type\": \"string\" },\n          \"vocabulary\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"isEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the thing is enabled and able to receive data\"\n    },\n    \"isSystemObject\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if this is a built-in ThingWorx system object\"\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"External identifier for mapping to physical device or asset\"\n    },\n    \"projectName\": {\n      \"type\": \"string\",\n      \"description\": \"ThingWorx project the thing belongs to\"\n    },\n    \"lastModifiedDate\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Last modification timestamp (epoch milliseconds\
  \ UTC)\"\n    }\n  },\n  \"required\": [\"name\", \"thingTemplate\"],\n  \"examples\": [\n    {\n      \"name\": \"CNC_Machine_Line3_Station7\",\n      \"description\": \"CNC Machining Center - Production Line 3, Station 7\",\n      \"thingTemplate\": \"GenericThingTemplate\",\n      \"thingShape\": \"CNCMachineShape\",\n      \"tags\": [\n        { \"name\": \"CNC\", \"vocabulary\": \"MachineType\" },\n        { \"name\": \"Line3\", \"vocabulary\": \"ProductionLine\" }\n      ],\n      \"isEnabled\": true,\n      \"isSystemObject\": false,\n      \"identifier\": \"ASSET-CNC-LINE3-007\",\n      \"projectName\": \"SmartFactoryProject\"\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ptc-thingworx/refs/heads/main/json-schema/ptc-thingworx-thing-schema.json
tags: []
title: PTC ThingWorx Thing
---
