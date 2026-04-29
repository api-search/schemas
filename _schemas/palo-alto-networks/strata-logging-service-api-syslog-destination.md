---
description: SyslogDestination schema from Palo Alto Networks Strata Logging Service API
layout: schema
name: SyslogDestination
properties_list:
- description: Unique identifier of the syslog destination.
  name: destination_id
  type: string
- description: Display name of the destination.
  name: name
  type: string
- description: Syslog server hostname or IP address.
  name: server
  type: string
- description: Syslog server port.
  name: port
  type: integer
- description: Transport protocol for syslog delivery.
  name: protocol
  type: string
- description: Syslog message format.
  name: format
  type: string
- description: Syslog facility value.
  name: facility
  type: string
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: created_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/strata-logging-service-api-syslog-destination-schema.json
slug: strata-logging-service-api-syslog-destination
source_filename: strata-logging-service-api-syslog-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SyslogDestination\",\n  \"description\": \"SyslogDestination schema from Palo Alto Networks Strata Logging Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-service-api-syslog-destination-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"destination_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the syslog destination.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the destination.\"\n    },\n    \"server\": {\n      \"type\": \"string\",\n      \"description\": \"Syslog server hostname or IP address.\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"Syslog server port.\"\n    },\n    \"protocol\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"UDP\",\n\
  \        \"TCP\",\n        \"SSL\"\n      ],\n      \"description\": \"Transport protocol for syslog delivery.\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"IETF\",\n        \"BSD\",\n        \"CSV\"\n      ],\n      \"description\": \"Syslog message format.\"\n    },\n    \"facility\": {\n      \"type\": \"string\",\n      \"description\": \"Syslog facility value.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-service-api-syslog-destination-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: SyslogDestination
---
