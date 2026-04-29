---
description: ConnectorGroupRequest schema from Palo Alto Networks ZTNA Connector API
layout: schema
name: ConnectorGroupRequest
properties_list:
- description: Display name for the connector group.
  name: name
  type: string
- description: Optional description of the connector group.
  name: description
  type: string
- description: Geographic region for this connector group.
  name: region
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/ztna-connector-api-connector-group-request-schema.json
slug: ztna-connector-api-connector-group-request
source_filename: ztna-connector-api-connector-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConnectorGroupRequest\",\n  \"description\": \"ConnectorGroupRequest schema from Palo Alto Networks ZTNA Connector API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-connector-group-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the connector group.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the connector group.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Geographic region for this connector group.\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-connector-group-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ConnectorGroupRequest
---
