---
description: A render host machine
layout: schema
name: Host
properties_list:
- description: Unique host identifier
  name: id
  type: string
- description: Hostname
  name: name
  type: string
- description: Host state
  name: state
  type: string
- description: Host lock state
  name: lock
  type: string
- description: Total CPU cores on the host
  name: totalCores
  type: integer
- description: Currently idle CPU cores
  name: idleCores
  type: integer
- description: Total memory in MB
  name: totalMemory
  type: integer
- description: Currently idle memory in MB
  name: idleMemory
  type: integer
- description: Current system load (percentage)
  name: load
  type: integer
provider_name: Academy Software Foundation
provider_slug: academy-software-foundation
schema_file: json-schema/opencue-host-schema.json
slug: opencue-host
source_filename: opencue-host-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/academy-software-foundation/refs/heads/main/json-schema/opencue-host-schema.json\",\n  \"title\": \"Host\",\n  \"description\": \"A render host machine\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique host identifier\",\n      \"example\": \"host-jkl012\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname\",\n      \"example\": \"render-host-001.studio.local\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Host state\",\n      \"example\": \"UP\",\n      \"enum\": [\n        \"UP\",\n        \"DOWN\",\n        \"REPAIR\"\n      ]\n    },\n    \"lock\": {\n      \"type\": \"string\",\n      \"description\": \"Host lock state\",\n      \"example\": \"OPEN\",\n      \"enum\": [\n        \"OPEN\",\n   \
  \     \"LOCKED\",\n        \"NIMBY_LOCKED\"\n      ]\n    },\n    \"totalCores\": {\n      \"type\": \"integer\",\n      \"description\": \"Total CPU cores on the host\",\n      \"example\": 64\n    },\n    \"idleCores\": {\n      \"type\": \"integer\",\n      \"description\": \"Currently idle CPU cores\",\n      \"example\": 32\n    },\n    \"totalMemory\": {\n      \"type\": \"integer\",\n      \"description\": \"Total memory in MB\",\n      \"example\": 131072\n    },\n    \"idleMemory\": {\n      \"type\": \"integer\",\n      \"description\": \"Currently idle memory in MB\",\n      \"example\": 65536\n    },\n    \"load\": {\n      \"type\": \"integer\",\n      \"description\": \"Current system load (percentage)\",\n      \"example\": 35\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/academy-software-foundation/refs/heads/main/json-schema/opencue-host-schema.json
tags:
- Animation
- Color Management
- Film
- Linux Foundation
- Open Source
- Rendering
- Standards
- Visual Effects
- VFX
title: Host
---
