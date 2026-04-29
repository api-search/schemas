---
description: Remote desktop connection configuration
layout: schema
name: Connection
properties_list:
- description: Unique connection identifier
  name: identifier
  type: string
- description: Human-readable connection name
  name: name
  type: string
- description: Remote desktop protocol
  name: protocol
  type: string
- description: Parent connection group identifier (ROOT for top-level)
  name: parentIdentifier
  type: string
- description: Number of active sessions for this connection
  name: activeConnections
  type: integer
- description: Protocol-specific connection parameters
  name: parameters
  type: object
provider_name: Apache Guacamole
provider_slug: apache-guacamole
schema_file: json-schema/guacamole-rest-connection-schema.json
slug: guacamole-rest-connection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/json-schema/guacamole-rest-connection-schema.json\",\n  \"title\": \"Connection\",\n  \"description\": \"Remote desktop connection configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"Unique connection identifier\",\n      \"example\": \"1\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable connection name\",\n      \"example\": \"My RDP Server\"\n    },\n    \"protocol\": {\n      \"type\": \"string\",\n      \"description\": \"Remote desktop protocol\",\n      \"enum\": [\n        \"rdp\",\n        \"vnc\",\n        \"ssh\",\n        \"telnet\",\n        \"kubernetes\"\n      ],\n      \"example\": \"rdp\"\n    },\n    \"parentIdentifier\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Parent connection group identifier (ROOT for top-level)\",\n      \"example\": \"ROOT\"\n    },\n    \"activeConnections\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of active sessions for this connection\",\n      \"example\": \"0\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"Protocol-specific connection parameters\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/json-schema/guacamole-rest-connection-schema.json
tags:
- Apache
- Open Source
- RDP
- Remote Access
- Remote Desktop
- SSH
- VNC
- Web Gateway
title: Connection
---
