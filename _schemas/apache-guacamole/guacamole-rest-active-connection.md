---
description: An active remote desktop session
layout: schema
name: ActiveConnection
properties_list:
- description: Unique active connection identifier
  name: identifier
  type: string
- description: Associated connection configuration ID
  name: connectionIdentifier
  type: string
- description: User who started the session
  name: username
  type: string
- description: Session start time in milliseconds since epoch
  name: startDate
  type: integer
- description: IP address of the connecting client
  name: remoteHost
  type: string
provider_name: Apache Guacamole
provider_slug: apache-guacamole
schema_file: json-schema/guacamole-rest-active-connection-schema.json
slug: guacamole-rest-active-connection
source_filename: guacamole-rest-active-connection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/json-schema/guacamole-rest-active-connection-schema.json\",\n  \"title\": \"ActiveConnection\",\n  \"description\": \"An active remote desktop session\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"Unique active connection identifier\",\n      \"example\": \"ac-500123\"\n    },\n    \"connectionIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"Associated connection configuration ID\",\n      \"example\": \"1\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"User who started the session\",\n      \"example\": \"jsmith\"\n    },\n    \"startDate\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Session start time in milliseconds since epoch\"\
  ,\n      \"example\": \"1718153645993\"\n    },\n    \"remoteHost\": {\n      \"type\": \"string\",\n      \"description\": \"IP address of the connecting client\",\n      \"example\": \"10.0.0.1\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/json-schema/guacamole-rest-active-connection-schema.json
tags:
- Apache
- Open Source
- RDP
- Remote Access
- Remote Desktop
- SSH
- VNC
- Web Gateway
title: ActiveConnection
---
