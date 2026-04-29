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
source_filename: route.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/apache-apisix/blob/main/json-schema/route.json\",\n  \"title\": \"Apache APISIX Route\",\n  \"description\": \"A Route defines rules to match client requests and specifies how to handle matched requests, including plugins and upstream configurations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"The request URI path. Supports path prefixes with wildcard.\"\n    },\n    \"uris\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A list of URIs for the route to match.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the route.\"\n    },\n    \"desc\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the route.\"\n    },\n    \"host\": {\n      \"\
  type\": \"string\",\n      \"description\": \"Host to match for the route.\"\n    },\n    \"hosts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A list of hosts for the route to match.\"\n    },\n    \"methods\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"GET\",\n          \"POST\",\n          \"PUT\",\n          \"DELETE\",\n          \"PATCH\",\n          \"HEAD\",\n          \"OPTIONS\",\n          \"CONNECT\",\n          \"TRACE\"\n        ]\n      },\n      \"description\": \"HTTP methods to match.\"\n    },\n    \"remote_addr\": {\n      \"type\": \"string\",\n      \"description\": \"Client IP address to match.\"\n    },\n    \"remote_addrs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A list of client IP addresses to match.\"\n    },\n    \"vars\": {\n      \"type\"\
  : \"array\",\n      \"description\": \"DSL expressions for matching request attributes.\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"default\": 0,\n      \"description\": \"Route priority for matching order. Higher value means higher priority.\"\n    },\n    \"plugins\": {\n      \"type\": \"object\",\n      \"description\": \"Plugin configuration. Key is the plugin name and value is the plugin config.\"\n    },\n    \"upstream\": {\n      \"$ref\": \"upstream.json\",\n      \"description\": \"Inline upstream configuration.\"\n    },\n    \"upstream_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of an existing upstream to use.\"\n    },\n    \"service_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of an existing service to bind to.\"\n    },\n    \"plugin_config_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of a plugin config to bind to.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"\
  additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key-value pairs for categorization.\"\n    },\n    \"timeout\": {\n      \"type\": \"object\",\n      \"description\": \"Timeout settings for upstream connections.\",\n      \"properties\": {\n        \"connect\": {\n          \"type\": \"number\",\n          \"default\": 60,\n          \"description\": \"Connection timeout in seconds.\"\n        },\n        \"send\": {\n          \"type\": \"number\",\n          \"default\": 60,\n          \"description\": \"Send timeout in seconds.\"\n        },\n        \"read\": {\n          \"type\": \"number\",\n          \"default\": 60,\n          \"description\": \"Read timeout in seconds.\"\n        }\n      }\n    },\n    \"enable_websocket\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable WebSocket proxying.\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"enum\": [0, 1],\n      \"default\": 1,\n      \"description\"\
  : \"Route status. 1 for enabled, 0 for disabled.\"\n    },\n    \"filter_func\": {\n      \"type\": \"string\",\n      \"description\": \"A Lua function string for custom filtering logic.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/json-schema/route.json
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
