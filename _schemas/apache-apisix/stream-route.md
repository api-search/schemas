---
description: A Stream Route is used for Layer 4 (TCP/UDP) traffic proxying.
layout: schema
name: Apache APISIX Stream Route
properties_list:
- description: Description of the stream route.
  name: desc
  type: string
- description: Client IP address to match.
  name: remote_addr
  type: string
- description: Server address to match.
  name: server_addr
  type: string
- description: Server port to match.
  name: server_port
  type: integer
- description: Server Name Indication value to match.
  name: sni
  type: string
- description: Plugin configuration for the stream route.
  name: plugins
  type: object
- description: Inline upstream configuration.
  name: upstream
  type: object
- description: ID of an existing upstream to use.
  name: upstream_id
  type: string
provider_name: Apache APISIX
provider_slug: apache-apisix
schema_file: json-schema/stream-route.json
slug: stream-route
tags:
- Apache
- API Gateway
- Cloud Native
- Kubernetes
- Lua
- NGINX
- Open Source
- Traffic Management
title: Apache APISIX Stream Route
---
