---
description: An active user session on the Oracle Essbase server. Sessions track connected users, their active application and database context, and any currently running requests such as calculations or data loads.
layout: schema
name: Oracle Essbase Session
properties_list:
- description: User name of the logged-in user who owns this session.
  name: userId
  type: string
- description: Unique numeric session identifier assigned by the server.
  name: sessionId
  type: string
- description: Number of seconds elapsed since the user logged in and the session began.
  name: loginTimeInSeconds
  type: string
- description: Name of the application the user is currently connected to, if any.
  name: application
  type: string
- description: Name of the database the user is currently connected to, if any.
  name: database
  type: string
- description: Number of seconds elapsed since the user connected to the active database.
  name: dbConnectTimeInSeconds
  type: string
- description: Type of the currently active request, such as calculation, data load, or restructure.
  name: request
  type: string
- description: Number of seconds the currently active request has been running.
  name: requestTimeInSeconds
  type: string
- description: Hostname or URL of the service from which the user connected.
  name: connectionSource
  type: string
- description: Current status of the active request.
  name: requestState
  type: string
provider_name: Oracle Essbase
provider_slug: oracle-essbase
schema_file: json-schema/oracle-essbase-session-schema.json
slug: oracle-essbase-session
source_filename: oracle-essbase-session-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"oracle-essbase-session-schema.json\",\n  \"title\": \"Oracle Essbase Session\",\n  \"description\": \"An active user session on the Oracle Essbase server. Sessions track connected users, their active application and database context, and any currently running requests such as calculations or data loads.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"User name of the logged-in user who owns this session.\"\n    },\n    \"sessionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique numeric session identifier assigned by the server.\"\n    },\n    \"loginTimeInSeconds\": {\n      \"type\": \"string\",\n      \"description\": \"Number of seconds elapsed since the user logged in and the session began.\"\n    },\n    \"application\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the application\
  \ the user is currently connected to, if any.\"\n    },\n    \"database\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the database the user is currently connected to, if any.\"\n    },\n    \"dbConnectTimeInSeconds\": {\n      \"type\": \"string\",\n      \"description\": \"Number of seconds elapsed since the user connected to the active database.\"\n    },\n    \"request\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the currently active request, such as calculation, data load, or restructure.\"\n    },\n    \"requestTimeInSeconds\": {\n      \"type\": \"string\",\n      \"description\": \"Number of seconds the currently active request has been running.\"\n    },\n    \"connectionSource\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname or URL of the service from which the user connected.\"\n    },\n    \"requestState\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the active request.\"\n    }\n\
  \  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/json-schema/oracle-essbase-session-schema.json
tags:
- Analytics
- Budgeting
- Business Intelligence
- Financial Consolidation
- Multi-Dimensional Database
- OLAP
- Planning
title: Oracle Essbase Session
---
