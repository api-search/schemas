---
description: ''
layout: schema
name: Connection
properties_list:
- description: The unique identifier for the connection.
  name: id
  type: string
- description: The type of connection (e.g., sqlserver, postgres).
  name: type
  type: string
- description: The address of the server for the connection.
  name: serverAddress
  type: string
- description: The port used for the connection.
  name: serverPort
  type: string
- description: The user name for the connection.
  name: userName
  type: string
- description: ''
  name: datasource
  type: object
provider_name: Tableau
provider_slug: tableau
schema_file: json-schema/tableau-rest-connection-schema.json
slug: tableau-rest-connection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Connection\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the connection.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of connection (e.g., sqlserver, postgres).\"\n    },\n    \"serverAddress\": {\n      \"type\": \"string\",\n      \"description\": \"The address of the server for the connection.\"\n    },\n    \"serverPort\": {\n      \"type\": \"string\",\n      \"description\": \"The port used for the connection.\"\n    },\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\": \"The user name for the connection.\"\n    },\n    \"datasource\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/json-schema/tableau-rest-connection-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
title: Connection
---
