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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/apache-apisix/blob/main/json-schema/service.json\",\n  \"title\": \"Apache APISIX Service\",\n  \"description\": \"A Service is an abstraction of an API and corresponds to an upstream service. It can be shared across routes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the service.\"\n    },\n    \"desc\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the service.\"\n    },\n    \"plugins\": {\n      \"type\": \"object\",\n      \"description\": \"Plugin configuration. Key is the plugin name and value is the plugin config.\"\n    },\n    \"upstream\": {\n      \"$ref\": \"upstream.json\",\n      \"description\": \"Inline upstream configuration.\"\n    },\n    \"upstream_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of\
  \ an existing upstream to use.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key-value pairs for categorization.\"\n    },\n    \"enable_websocket\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable WebSocket proxying.\"\n    },\n    \"hosts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A list of hosts for the service.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/json-schema/service.json
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
