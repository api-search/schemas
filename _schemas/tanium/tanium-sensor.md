---
description: Represents a sensor in the Tanium platform. Sensors are scripts that run on endpoints to collect specific data points such as installed software, running processes, network configuration, or security posture.
layout: schema
name: Tanium Sensor
properties_list:
- description: Unique numeric identifier for the sensor
  name: id
  type: integer
- description: Sensor name used in questions
  name: name
  type: string
- description: Hash identifier for the sensor
  name: hash
  type: integer
- description: Human-readable description of what the sensor collects
  name: description
  type: string
- description: Category grouping for the sensor
  name: category
  type: string
- description: Maximum age in seconds for cached sensor results before re-execution
  name: maxAgeSeconds
  type: integer
- description: Content set the sensor belongs to
  name: contentSet
  type: object
- description: Platform-specific query scripts
  name: queries
  type: array
- description: Configurable parameters for the sensor
  name: parameters
  type: array
- description: Last modification timestamp
  name: modTime
  type: string
- description: Creation timestamp
  name: creationTime
  type: string
provider_name: Tanium
provider_slug: tanium
schema_file: json-schema/tanium-sensor-schema.json
slug: tanium-sensor
source_filename: tanium-sensor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/tanium/blob/main/json-schema/tanium-sensor-schema.json\",\n  \"title\": \"Tanium Sensor\",\n  \"description\": \"Represents a sensor in the Tanium platform. Sensors are scripts that run on endpoints to collect specific data points such as installed software, running processes, network configuration, or security posture.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier for the sensor\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Sensor name used in questions\"\n    },\n    \"hash\": {\n      \"type\": \"integer\",\n      \"description\": \"Hash identifier for the sensor\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of what the sensor collects\"\n    },\n    \"category\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Category grouping for the sensor\"\n    },\n    \"maxAgeSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum age in seconds for cached sensor results before re-execution\"\n    },\n    \"contentSet\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Content set identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Content set name\"\n        }\n      },\n      \"description\": \"Content set the sensor belongs to\"\n    },\n    \"queries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"platform\": {\n            \"type\": \"string\",\n            \"description\": \"Target platform (Windows, Linux, Mac, Solaris, AIX)\"\n          },\n          \"script\": {\n            \"type\": \"string\"\
  ,\n            \"description\": \"Script content that runs on the endpoint\"\n          },\n          \"scriptType\": {\n            \"type\": \"string\",\n            \"description\": \"Script language (VBScript, PowerShell, UnixShell, Python)\"\n          }\n        }\n      },\n      \"description\": \"Platform-specific query scripts\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\",\n            \"description\": \"Parameter key name\"\n          },\n          \"defaultValue\": {\n            \"type\": \"string\",\n            \"description\": \"Default parameter value\"\n          }\n        }\n      },\n      \"description\": \"Configurable parameters for the sensor\"\n    },\n    \"modTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp\"\n    },\n    \"creationTime\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp\"\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/json-schema/tanium-sensor-schema.json
tags:
- Compliance
- Endpoint Management
- Patch Management
- Security
- Threat Detection
- Unified Endpoint Management
title: Tanium Sensor
---
