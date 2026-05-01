---
description: JSON Schema for Fiber web framework application configuration (fiber.Config).
layout: schema
name: Fiber App Configuration
properties_list:
- description: Enable prefork mode to spawn multiple processes.
  name: Prefork
  type: boolean
- description: Value for the Server HTTP header.
  name: ServerHeader
  type: string
- description: Treat /foo and /foo/ as different routes.
  name: StrictRouting
  type: boolean
- description: Enable case-sensitive routing.
  name: CaseSensitive
  type: boolean
- description: Return immutable context values.
  name: Immutable
  type: boolean
- description: Unescape route path before matching.
  name: UnescapePath
  type: boolean
- description: Enable ETag header generation.
  name: ETag
  type: boolean
- description: Maximum request body size in bytes (default 4MB).
  name: BodyLimit
  type: integer
- description: Maximum number of concurrent connections.
  name: Concurrency
  type: integer
- description: Read timeout duration (e.g., 5s, 1m).
  name: ReadTimeout
  type: string
- description: Write timeout duration.
  name: WriteTimeout
  type: string
- description: Idle connection timeout duration.
  name: IdleTimeout
  type: string
- description: Per-connection read buffer size in bytes.
  name: ReadBufferSize
  type: integer
- description: Per-connection write buffer size in bytes.
  name: WriteBufferSize
  type: integer
- description: Suffix for compressed static files.
  name: CompressedFileSuffix
  type: string
- description: Header to use for proxy IP (e.g., X-Forwarded-For).
  name: ProxyHeader
  type: string
- description: Reject all non-GET requests.
  name: GETOnly
  type: boolean
- description: Disable keep-alive connections.
  name: DisableKeepalive
  type: boolean
- description: Disable default Date header.
  name: DisableDefaultDate
  type: boolean
- description: Disable default Content-Type header.
  name: DisableDefaultContentType
  type: boolean
- description: Disable automatic header name normalization.
  name: DisableHeaderNormalizing
  type: boolean
- description: Disable startup banner message.
  name: DisableStartupMessage
  type: boolean
- description: Application name.
  name: AppName
  type: string
- description: Enable streaming request body handling.
  name: StreamRequestBody
  type: boolean
- description: Enable trusted proxy checking.
  name: EnableTrustedProxyCheck
  type: boolean
- description: List of trusted proxy IP addresses/ranges.
  name: TrustedProxies
  type: array
- description: Network type for the listener.
  name: Network
  type: string
- description: Print all registered routes on startup.
  name: EnablePrintRoutes
  type: boolean
provider_name: Fiber
provider_slug: fiber
schema_file: json-schema/fiber-configuration.json
slug: fiber-configuration
source_filename: fiber-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/fiber/json-schema/fiber-configuration.json\",\n  \"title\": \"Fiber App Configuration\",\n  \"description\": \"JSON Schema for Fiber web framework application configuration (fiber.Config).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Prefork\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Enable prefork mode to spawn multiple processes.\"\n    },\n    \"ServerHeader\": {\n      \"type\": \"string\",\n      \"description\": \"Value for the Server HTTP header.\"\n    },\n    \"StrictRouting\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Treat /foo and /foo/ as different routes.\"\n    },\n    \"CaseSensitive\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Enable case-sensitive routing.\"\n    },\n    \"Immutable\": {\n      \"type\"\
  : \"boolean\",\n      \"default\": false,\n      \"description\": \"Return immutable context values.\"\n    },\n    \"UnescapePath\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Unescape route path before matching.\"\n    },\n    \"ETag\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Enable ETag header generation.\"\n    },\n    \"BodyLimit\": {\n      \"type\": \"integer\",\n      \"default\": 4194304,\n      \"description\": \"Maximum request body size in bytes (default 4MB).\"\n    },\n    \"Concurrency\": {\n      \"type\": \"integer\",\n      \"default\": 262144,\n      \"description\": \"Maximum number of concurrent connections.\"\n    },\n    \"ReadTimeout\": {\n      \"type\": \"string\",\n      \"description\": \"Read timeout duration (e.g., 5s, 1m).\"\n    },\n    \"WriteTimeout\": {\n      \"type\": \"string\",\n      \"description\": \"Write timeout duration.\"\n    },\n    \"IdleTimeout\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Idle connection timeout duration.\"\n    },\n    \"ReadBufferSize\": {\n      \"type\": \"integer\",\n      \"default\": 4096,\n      \"description\": \"Per-connection read buffer size in bytes.\"\n    },\n    \"WriteBufferSize\": {\n      \"type\": \"integer\",\n      \"default\": 4096,\n      \"description\": \"Per-connection write buffer size in bytes.\"\n    },\n    \"CompressedFileSuffix\": {\n      \"type\": \"string\",\n      \"default\": \".fiber.gz\",\n      \"description\": \"Suffix for compressed static files.\"\n    },\n    \"ProxyHeader\": {\n      \"type\": \"string\",\n      \"description\": \"Header to use for proxy IP (e.g., X-Forwarded-For).\"\n    },\n    \"GETOnly\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Reject all non-GET requests.\"\n    },\n    \"DisableKeepalive\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Disable keep-alive\
  \ connections.\"\n    },\n    \"DisableDefaultDate\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Disable default Date header.\"\n    },\n    \"DisableDefaultContentType\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Disable default Content-Type header.\"\n    },\n    \"DisableHeaderNormalizing\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Disable automatic header name normalization.\"\n    },\n    \"DisableStartupMessage\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Disable startup banner message.\"\n    },\n    \"AppName\": {\n      \"type\": \"string\",\n      \"description\": \"Application name.\"\n    },\n    \"StreamRequestBody\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Enable streaming request body handling.\"\n    },\n    \"EnableTrustedProxyCheck\": {\n      \"type\": \"\
  boolean\",\n      \"default\": false,\n      \"description\": \"Enable trusted proxy checking.\"\n    },\n    \"TrustedProxies\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"List of trusted proxy IP addresses/ranges.\"\n    },\n    \"Network\": {\n      \"type\": \"string\",\n      \"enum\": [\"tcp\", \"tcp4\", \"tcp6\"],\n      \"default\": \"tcp4\",\n      \"description\": \"Network type for the listener.\"\n    },\n    \"EnablePrintRoutes\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Print all registered routes on startup.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fiber/refs/heads/main/json-schema/fiber-configuration.json
tags:
- Microservices
title: Fiber App Configuration
---
