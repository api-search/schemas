---
description: Guacamole user account
layout: schema
name: User
properties_list:
- description: Unique username
  name: username
  type: string
- description: User password (write-only)
  name: password
  type: string
- description: Additional user attributes
  name: attributes
  type: object
- description: Timestamp of last user activity in milliseconds
  name: lastActive
  type: integer
provider_name: Apache Guacamole
provider_slug: apache-guacamole
schema_file: json-schema/guacamole-rest-user-schema.json
slug: guacamole-rest-user
tags:
- Apache
- Open Source
- RDP
- Remote Access
- Remote Desktop
- SSH
- VNC
- Web Gateway
title: User
---
