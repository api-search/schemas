---
description: A Route defines rules to match client requests and specifies how to handle matched requests, including plugins and upstream configurations.
layout: schema
name: Apache APISIX Route
properties_list:
- description: The request URI path. Supports path prefixes with wildcard.
  name: uri
  type: string
- description: A list of URIs for the route to match.
  name: uris
  type: array
- description: Human-readable name for the route.
  name: name
  type: string
- description: Description of the route.
  name: desc
  type: string
- description: Host to match for the route.
  name: host
  type: string
- description: A list of hosts for the route to match.
  name: hosts
  type: array
- description: HTTP methods to match.
  name: methods
  type: array
- description: Client IP address to match.
  name: remote_addr
  type: string
- description: A list of client IP addresses to match.
  name: remote_addrs
  type: array
- description: DSL expressions for matching request attributes.
  name: vars
  type: array
- description: Route priority for matching order. Higher value means higher priority.
  name: priority
  type: integer
- description: Plugin configuration. Key is the plugin name and value is the plugin config.
  name: plugins
  type: object
- description: Inline upstream configuration.
  name: upstream
  type: object
- description: ID of an existing upstream to use.
  name: upstream_id
  type: string
- description: ID of an existing service to bind to.
  name: service_id
  type: string
- description: ID of a plugin config to bind to.
  name: plugin_config_id
  type: string
- description: Key-value pairs for categorization.
  name: labels
  type: object
- description: Timeout settings for upstream connections.
  name: timeout
  type: object
- description: Enable WebSocket proxying.
  name: enable_websocket
  type: boolean
- description: Route status. 1 for enabled, 0 for disabled.
  name: status
  type: integer
- description: A Lua function string for custom filtering logic.
  name: filter_func
  type: string
provider_name: Apache APISIX
provider_slug: apache-apisix
schema_file: json-schema/route.json
slug: route
tags:
- Apache
- API Gateway
- Cloud Native
- Kubernetes
- Lua
- NGINX
- Open Source
- Traffic Management
title: Apache APISIX Route
---
