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
tags:
- Apache
- Load Balancer
- Open Source
- Proxy
- Reverse Proxy
- Web Server
title: ServerStatus
---
