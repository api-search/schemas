---
description: A group organizing connections and other connection groups
layout: schema
name: ConnectionGroup
properties_list:
- description: Unique group identifier
  name: identifier
  type: string
- description: Group name
  name: name
  type: string
- description: Group type (ORGANIZATIONAL or BALANCING)
  name: type
  type: string
- description: Parent group identifier
  name: parentIdentifier
  type: string
- description: Total active connections in this group
  name: activeConnections
  type: integer
provider_name: Apache Guacamole
provider_slug: apache-guacamole
schema_file: json-schema/guacamole-rest-connection-group-schema.json
slug: guacamole-rest-connection-group
tags:
- Apache
- Open Source
- RDP
- Remote Access
- Remote Desktop
- SSH
- VNC
- Web Gateway
title: ConnectionGroup
---
