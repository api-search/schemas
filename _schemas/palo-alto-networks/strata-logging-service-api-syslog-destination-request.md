---
description: SyslogDestinationRequest schema from Palo Alto Networks Strata Logging Service API
layout: schema
name: SyslogDestinationRequest
properties_list:
- description: Display name for this syslog destination.
  name: name
  type: string
- description: Syslog server hostname or IP address.
  name: server
  type: string
- description: Syslog server port number.
  name: port
  type: integer
- description: Transport protocol.
  name: protocol
  type: string
- description: ''
  name: format
  type: string
- description: ''
  name: facility
  type: string
- description: ''
  name: enabled
  type: boolean
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/strata-logging-service-api-syslog-destination-request-schema.json
slug: strata-logging-service-api-syslog-destination-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SyslogDestinationRequest\",\n  \"description\": \"SyslogDestinationRequest schema from Palo Alto Networks Strata Logging Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-service-api-syslog-destination-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for this syslog destination.\"\n    },\n    \"server\": {\n      \"type\": \"string\",\n      \"description\": \"Syslog server hostname or IP address.\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 65535,\n      \"description\": \"Syslog server port number.\"\n    },\n    \"protocol\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"UDP\",\n        \"TCP\",\n        \"SSL\"\n      ],\n   \
  \   \"description\": \"Transport protocol.\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"IETF\",\n        \"BSD\",\n        \"CSV\"\n      ],\n      \"default\": \"IETF\"\n    },\n    \"facility\": {\n      \"type\": \"string\",\n      \"default\": \"LOG_USER\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"default\": true\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"server\",\n    \"port\",\n    \"protocol\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-service-api-syslog-destination-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: SyslogDestinationRequest
---
