---
description: Base request structure for all Reolink Camera HTTP API commands sent as JSON POST to /cgi-bin/api.cgi.
layout: schema
name: Reolink Command Request
properties_list:
- description: The API command name to execute (e.g., Login, GetDevInfo, PtzCtrl)
  name: cmd
  type: string
- description: 'Action type: 0 for get/read operations, 1 for set/write operations'
  name: action
  type: integer
- description: Command-specific parameters
  name: param
  type: object
provider_name: Reolink
provider_slug: reolink
schema_file: json-schema/command-request.json
slug: command-request
source_filename: command-request.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"command-request.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Reolink Command Request\",\n  \"description\": \"Base request structure for all Reolink Camera HTTP API commands sent as JSON POST to /cgi-bin/api.cgi.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cmd\": {\n      \"type\": \"string\",\n      \"description\": \"The API command name to execute (e.g., Login, GetDevInfo, PtzCtrl)\"\n    },\n    \"action\": {\n      \"type\": \"integer\",\n      \"description\": \"Action type: 0 for get/read operations, 1 for set/write operations\",\n      \"enum\": [0, 1]\n    },\n    \"param\": {\n      \"type\": \"object\",\n      \"description\": \"Command-specific parameters\"\n    }\n  },\n  \"required\": [\"cmd\", \"action\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/json-schema/command-request.json
tags:
- IoT
- Security Cameras
- Surveillance
- Smart Home
- AI Detection
title: Reolink Command Request
---
