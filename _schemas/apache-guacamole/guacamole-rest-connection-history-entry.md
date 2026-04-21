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
