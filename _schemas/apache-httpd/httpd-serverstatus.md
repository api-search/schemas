---
description: Apache HTTP Server status information from mod_status
layout: schema
name: ServerStatus
properties_list:
- description: Apache server version string
  name: ServerVersion
  type: string
- description: Multi-processing module in use
  name: ServerMPM
  type: string
- description: Server uptime in seconds
  name: ServerUptimeSeconds
  type: integer
- description: 1-minute load average
  name: Load1
  type: number
- description: 5-minute load average
  name: Load5
  type: number
- description: 15-minute load average
  name: Load15
  type: number
- description: Requests per second
  name: ReqPerSec
  type: number
- description: Bytes transferred per second
  name: BytesPerSec
  type: number
- description: Number of busy worker threads
  name: BusyWorkers
  type: integer
- description: Number of idle worker threads
  name: IdleWorkers
  type: integer
- description: Worker state scoreboard string
  name: Scoreboard
  type: string
provider_name: Apache HTTP Server
provider_slug: apache-httpd
schema_file: json-schema/httpd-serverstatus-schema.json
slug: httpd-serverstatus
source_filename: httpd-serverstatus-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-httpd/json-schema/httpd-serverstatus-schema.json\",\n  \"title\": \"ServerStatus\",\n  \"type\": \"object\",\n  \"description\": \"Apache HTTP Server status information from mod_status\",\n  \"properties\": {\n    \"ServerVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Apache server version string\",\n      \"example\": \"Apache/2.4.57 (Unix)\"\n    },\n    \"ServerMPM\": {\n      \"type\": \"string\",\n      \"description\": \"Multi-processing module in use\",\n      \"example\": \"event\"\n    },\n    \"ServerUptimeSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Server uptime in seconds\",\n      \"example\": 86400\n    },\n    \"Load1\": {\n      \"type\": \"number\",\n      \"description\": \"1-minute load average\",\n      \"example\": 0.12\n    },\n    \"Load5\": {\n      \"type\": \"number\",\n      \"description\"\
  : \"5-minute load average\",\n      \"example\": 0.09\n    },\n    \"Load15\": {\n      \"type\": \"number\",\n      \"description\": \"15-minute load average\",\n      \"example\": 0.08\n    },\n    \"ReqPerSec\": {\n      \"type\": \"number\",\n      \"description\": \"Requests per second\",\n      \"example\": 142.3\n    },\n    \"BytesPerSec\": {\n      \"type\": \"number\",\n      \"description\": \"Bytes transferred per second\",\n      \"example\": 512000\n    },\n    \"BusyWorkers\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of busy worker threads\",\n      \"example\": 10\n    },\n    \"IdleWorkers\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of idle worker threads\",\n      \"example\": 6\n    },\n    \"Scoreboard\": {\n      \"type\": \"string\",\n      \"description\": \"Worker state scoreboard string\",\n      \"example\": \"___________W_______\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-httpd/refs/heads/main/json-schema/httpd-serverstatus-schema.json
tags:
- Apache
- Load Balancer
- Open Source
- Proxy
- Reverse Proxy
- Web Server
title: ServerStatus
---
