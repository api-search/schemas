---
description: Standard response structure returned by all Reolink Camera HTTP API commands.
layout: schema
name: Reolink Command Response
properties_list:
- description: The command that was executed
  name: cmd
  type: string
- description: Response code where 0 indicates success
  name: code
  type: integer
- description: Command-specific response data
  name: value
  type: object
- description: Error information when the command fails
  name: error
  type: object
provider_name: Reolink
provider_slug: reolink
schema_file: json-schema/command-response.json
slug: command-response
source_filename: command-response.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"command-response.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Reolink Command Response\",\n  \"description\": \"Standard response structure returned by all Reolink Camera HTTP API commands.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cmd\": {\n      \"type\": \"string\",\n      \"description\": \"The command that was executed\"\n    },\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"Response code where 0 indicates success\"\n    },\n    \"value\": {\n      \"type\": \"object\",\n      \"description\": \"Command-specific response data\"\n    },\n    \"error\": {\n      \"type\": \"object\",\n      \"description\": \"Error information when the command fails\",\n      \"properties\": {\n        \"rspCode\": {\n          \"type\": \"integer\",\n          \"description\": \"Error response code\"\n        },\n        \"detail\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Human-readable error detail message\"\n        }\n      }\n    }\n  },\n  \"required\": [\"cmd\", \"code\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/json-schema/command-response.json
tags:
- IoT
- Security Cameras
- Surveillance
- Smart Home
- AI Detection
title: Reolink Command Response
---
