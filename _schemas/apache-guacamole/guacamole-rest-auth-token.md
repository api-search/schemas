---
description: Authentication token response from Guacamole login
layout: schema
name: AuthToken
properties_list:
- description: Session authentication token
  name: authToken
  type: string
- description: Authenticated username
  name: username
  type: string
- description: Default data source identifier
  name: dataSource
  type: string
- description: List of available data source identifiers
  name: availableDataSources
  type: array
provider_name: Apache Guacamole
provider_slug: apache-guacamole
schema_file: json-schema/guacamole-rest-auth-token-schema.json
slug: guacamole-rest-auth-token
tags:
- Apache
- Open Source
- RDP
- Remote Access
- Remote Desktop
- SSH
- VNC
- Web Gateway
title: AuthToken
---
