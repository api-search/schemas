---
description: ConnectorGroup schema from Palo Alto Networks ZTNA Connector API
layout: schema
name: ConnectorGroup
properties_list:
- description: Unique identifier of the connector group.
  name: group_id
  type: string
- description: Display name of the connector group.
  name: name
  type: string
- description: Description of the connector group's purpose.
  name: description
  type: string
- description: Number of connectors in this group.
  name: connector_count
  type: integer
- description: Primary geographic region for this connector group.
  name: region
  type: string
- description: ''
  name: created_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/ztna-connector-api-connector-group-schema.json
slug: ztna-connector-api-connector-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConnectorGroup\",\n  \"description\": \"ConnectorGroup schema from Palo Alto Networks ZTNA Connector API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-connector-group-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"group_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the connector group.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the connector group.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the connector group's purpose.\"\n    },\n    \"connector_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of connectors in this group.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Primary\
  \ geographic region for this connector group.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-connector-group-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ConnectorGroup
---
