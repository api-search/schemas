---
description: A Service is an abstraction of an API and corresponds to an upstream service. It can be shared across routes.
layout: schema
name: Apache APISIX Service
properties_list:
- description: Human-readable name for the service.
  name: name
  type: string
- description: Description of the service.
  name: desc
  type: string
- description: Plugin configuration. Key is the plugin name and value is the plugin config.
  name: plugins
  type: object
- description: Inline upstream configuration.
  name: upstream
  type: object
- description: ID of an existing upstream to use.
  name: upstream_id
  type: string
- description: Key-value pairs for categorization.
  name: labels
  type: object
- description: Enable WebSocket proxying.
  name: enable_websocket
  type: boolean
- description: A list of hosts for the service.
  name: hosts
  type: array
provider_name: Apache APISIX
provider_slug: apache-apisix
schema_file: json-schema/service.json
slug: service
tags:
- Apache
- API Gateway
- Cloud Native
- Kubernetes
- Lua
- NGINX
- Open Source
- Traffic Management
title: Apache APISIX Service
---
