---
description: ConnectorRequest schema from Palo Alto Networks ZTNA Connector API
layout: schema
name: ConnectorRequest
properties_list:
- description: Display name for the connector.
  name: name
  type: string
- description: ID of the connector group to assign the connector to.
  name: group_id
  type: string
- description: Optional description of the connector's purpose or location.
  name: description
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/ztna-connector-api-connector-request-schema.json
slug: ztna-connector-api-connector-request
source_filename: ztna-connector-api-connector-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConnectorRequest\",\n  \"description\": \"ConnectorRequest schema from Palo Alto Networks ZTNA Connector API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-connector-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the connector.\"\n    },\n    \"group_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the connector group to assign the connector to.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the connector's purpose or location.\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"group_id\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-connector-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ConnectorRequest
---
