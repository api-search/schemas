---
description: Historical record of a completed or active connection
layout: schema
name: ConnectionHistoryEntry
properties_list:
- description: History entry identifier
  name: identifier
  type: string
- description: Associated connection ID
  name: connectionIdentifier
  type: string
- description: Name of the connection
  name: connectionName
  type: string
- description: Username who made the connection
  name: username
  type: string
- description: Connection start time in milliseconds
  name: startDate
  type: integer
- description: Connection end time in milliseconds (null if still active)
  name: endDate
  type: integer
provider_name: Apache Guacamole
provider_slug: apache-guacamole
schema_file: json-schema/guacamole-rest-connection-history-entry-schema.json
slug: guacamole-rest-connection-history-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/json-schema/guacamole-rest-connection-history-entry-schema.json\",\n  \"title\": \"ConnectionHistoryEntry\",\n  \"description\": \"Historical record of a completed or active connection\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"History entry identifier\",\n      \"example\": \"hist-500123\"\n    },\n    \"connectionIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"Associated connection ID\",\n      \"example\": \"1\"\n    },\n    \"connectionName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the connection\",\n      \"example\": \"My RDP Server\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Username who made the connection\",\n      \"example\": \"jsmith\"\
  \n    },\n    \"startDate\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Connection start time in milliseconds\",\n      \"example\": \"1718153645993\"\n    },\n    \"endDate\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Connection end time in milliseconds (null if still active)\",\n      \"example\": \"1718157245993\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/json-schema/guacamole-rest-connection-history-entry-schema.json
tags:
- Apache
- Open Source
- RDP
- Remote Access
- Remote Desktop
- SSH
- VNC
- Web Gateway
title: ConnectionHistoryEntry
---
