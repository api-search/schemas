---
description: A Route defines rules to match client requests. Each Route is associated with a Service, and a Service may have multiple Routes. When a request matches a Route, Kong proxies the request to the associated Service.
layout: schema
name: Route
properties_list:
- description: The unique identifier of the Route.
  name: id
  type: string
- description: An optional human-readable name for the Route.
  name: name
  type: string
- description: An array of the protocols this Route should allow.
  name: protocols
  type: array
- description: A list of HTTP methods that match this Route.
  name: methods
  type: array
- description: A list of domain names that match this Route.
  name: hosts
  type: array
- description: A list of paths that match this Route.
  name: paths
  type: array
- description: One or more lists of values indexed by header name that will cause this Route to match if present in the request.
  name: headers
  type: object
- description: A list of SNIs that match this Route when using stream routing.
  name: snis
  type: array
- description: A list of IP sources of incoming connections that match this Route (stream routing).
  name: sources
  type: array
- description: A list of IP destinations of incoming connections that match this Route (stream routing).
  name: destinations
  type: array
- description: The status code Kong responds with when all properties of a Route match except the protocol.
  name: https_redirect_status_code
  type: integer
- description: A number used to choose which Route resolves a given request when several Routes match it using regexes simultaneously.
  name: regex_priority
  type: integer
- description: When matching a Route via one of the paths, strip the matching prefix from the upstream request URL.
  name: strip_path
  type: boolean
- description: Controls how the Service path, Route path, and requested path are combined when sending a request to the upstream.
  name: path_handling
  type: string
- description: When matching a Route via one of the hosts domain names, use the request Host header in the upstream request headers.
  name: preserve_host
  type: boolean
- description: Whether to enable request body buffering.
  name: request_buffering
  type: boolean
- description: Whether to enable response body buffering.
  name: response_buffering
  type: boolean
- description: An optional set of strings for grouping and filtering.
  name: tags
  type: array
- description: The Service this Route is associated with.
  name: service
  type: object
- description: The router expression for the Route (expressions router mode).
  name: expression
  type: string
- description: The priority of the Route in expressions router mode.
  name: priority
  type: integer
- description: Unix epoch timestamp of when the entity was created.
  name: created_at
  type: integer
- description: Unix epoch timestamp of when the entity was last updated.
  name: updated_at
  type: integer
provider_name: Kong
provider_slug: kong
schema_file: json-schema/kong-gateway-admin-route-schema.json
slug: kong-gateway-admin-route
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Route\",\n  \"type\": \"object\",\n  \"description\": \"A Route defines rules to match client requests. Each Route is associated with a Service, and a Service may have multiple Routes. When a request matches a Route, Kong proxies the request to the associated Service.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the Route.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"An optional human-readable name for the Route.\"\n    },\n    \"protocols\": {\n      \"type\": \"array\",\n      \"description\": \"An array of the protocols this Route should allow.\"\n    },\n    \"methods\": {\n      \"type\": \"array\",\n      \"description\": \"A list of HTTP methods that match this Route.\"\n    },\n    \"hosts\": {\n      \"type\": \"array\",\n      \"description\": \"A list of domain names that\
  \ match this Route.\"\n    },\n    \"paths\": {\n      \"type\": \"array\",\n      \"description\": \"A list of paths that match this Route.\"\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"One or more lists of values indexed by header name that will cause this Route to match if present in the request.\"\n    },\n    \"snis\": {\n      \"type\": \"array\",\n      \"description\": \"A list of SNIs that match this Route when using stream routing.\"\n    },\n    \"sources\": {\n      \"type\": \"array\",\n      \"description\": \"A list of IP sources of incoming connections that match this Route (stream routing).\"\n    },\n    \"destinations\": {\n      \"type\": \"array\",\n      \"description\": \"A list of IP destinations of incoming connections that match this Route (stream routing).\"\n    },\n    \"https_redirect_status_code\": {\n      \"type\": \"integer\",\n      \"description\": \"The status code Kong responds with when all properties of a Route\
  \ match except the protocol.\"\n    },\n    \"regex_priority\": {\n      \"type\": \"integer\",\n      \"description\": \"A number used to choose which Route resolves a given request when several Routes match it using regexes simultaneously.\"\n    },\n    \"strip_path\": {\n      \"type\": \"boolean\",\n      \"description\": \"When matching a Route via one of the paths, strip the matching prefix from the upstream request URL.\"\n    },\n    \"path_handling\": {\n      \"type\": \"string\",\n      \"description\": \"Controls how the Service path, Route path, and requested path are combined when sending a request to the upstream.\"\n    },\n    \"preserve_host\": {\n      \"type\": \"boolean\",\n      \"description\": \"When matching a Route via one of the hosts domain names, use the request Host header in the upstream request headers.\"\n    },\n    \"request_buffering\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable request body buffering.\"\n    },\n  \
  \  \"response_buffering\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable response body buffering.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"An optional set of strings for grouping and filtering.\"\n    },\n    \"service\": {\n      \"type\": \"object\",\n      \"description\": \"The Service this Route is associated with.\"\n    },\n    \"expression\": {\n      \"type\": \"string\",\n      \"description\": \"The router expression for the Route (expressions router mode).\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"The priority of the Route in expressions router mode.\"\n    },\n    \"created_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix epoch timestamp of when the entity was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix epoch timestamp of when the entity was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/json-schema/kong-gateway-admin-route-schema.json
tags:
- API Gateway
- Lua
- NGINX
- Open Source
title: Route
---
