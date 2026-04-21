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
