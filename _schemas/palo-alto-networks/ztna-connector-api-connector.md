---
description: Connector schema from Palo Alto Networks ZTNA Connector API
layout: schema
name: Connector
properties_list:
- description: Unique identifier of the connector.
  name: connector_id
  type: string
- description: Display name of the connector.
  name: name
  type: string
- description: ID of the connector group this connector belongs to.
  name: group_id
  type: string
- description: Current health status of the connector.
  name: status
  type: string
- description: Installed connector software version.
  name: version
  type: string
- description: Hostname of the system where the connector is installed.
  name: hostname
  type: string
- description: IP address of the connector host.
  name: ip_address
  type: string
- description: Geographic region where the connector is deployed.
  name: region
  type: string
- description: Timestamp of the connector's most recent heartbeat.
  name: last_seen_at
  type: string
- description: ''
  name: created_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/ztna-connector-api-connector-schema.json
slug: ztna-connector-api-connector
source_filename: ztna-connector-api-connector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Connector\",\n  \"description\": \"Connector schema from Palo Alto Networks ZTNA Connector API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-connector-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connector_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the connector.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the connector.\"\n    },\n    \"group_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the connector group this connector belongs to.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"connected\",\n        \"disconnected\",\n        \"upgrading\",\n        \"error\"\n      ],\n      \"description\": \"Current health status of the connector.\"\
  \n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Installed connector software version.\"\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname of the system where the connector is installed.\"\n    },\n    \"ip_address\": {\n      \"type\": \"string\",\n      \"description\": \"IP address of the connector host.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Geographic region where the connector is deployed.\"\n    },\n    \"last_seen_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the connector's most recent heartbeat.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-connector-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Connector
---
