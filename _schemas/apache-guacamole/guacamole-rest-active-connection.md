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
