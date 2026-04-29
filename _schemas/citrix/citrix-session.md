---
description: Represents an active user session on a Citrix virtual desktop or application, including connection state and hosting machine information.
layout: schema
name: Citrix Session
properties_list:
- description: Unique identifier for the session
  name: id
  type: string
- description: Username of the session owner
  name: userName
  type: string
- description: Current session state
  name: state
  type: string
- description: When the session was established
  name: startTime
  type: string
- description: Name of the machine hosting the session
  name: machineName
  type: string
- description: Name of the client device connected to the session
  name: clientName
  type: string
- description: Applications currently running in the session
  name: applicationNames
  type: array
provider_name: Citrix
provider_slug: citrix
schema_file: json-schema/citrix-session-schema.json
slug: citrix-session
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.citrix.com/schemas/citrix/session.json\",\n  \"title\": \"Citrix Session\",\n  \"description\": \"Represents an active user session on a Citrix virtual desktop or application, including connection state and hosting machine information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the session\"\n    },\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the session owner\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"Active\", \"Disconnected\"],\n      \"description\": \"Current session state\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the session was established\"\n    },\n    \"machineName\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Name of the machine hosting the session\"\n    },\n    \"clientName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the client device connected to the session\"\n    },\n    \"applicationNames\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Applications currently running in the session\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/citrix/refs/heads/main/json-schema/citrix-session-schema.json
tags:
- Application Delivery
- Desktop-As-A-Service
- Networking
- Virtualization
- Workspace
title: Citrix Session
---
