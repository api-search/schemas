---
description: JSON Schema for hapi server configuration options passed to Hapi.server().
layout: schema
name: hapi Server Configuration
properties_list:
- description: Public hostname or IP address.
  name: host
  type: string
- description: TCP port to listen on.
  name: port
  type: integer
- description: Hostname or IP address to bind to (defaults to host).
  name: address
  type: string
- description: Whether to automatically start listening.
  name: autoListen
  type: boolean
- description: TLS configuration.
  name: tls
  type: object
- description: Default route configuration.
  name: routes
  type: object
- description: Server-side cache provider configuration.
  name: cache
  type: object
- description: Compression settings.
  name: compression
  type: object
- description: Debug logging configuration.
  name: debug
  type: object
- description: Server load monitoring configuration.
  name: load
  type: object
provider_name: Hapi
provider_slug: hapi
schema_file: json-schema/hapi-server-configuration.json
slug: hapi-server-configuration
source_filename: hapi-server-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/hapi/json-schema/hapi-server-configuration.json\",\n  \"title\": \"hapi Server Configuration\",\n  \"description\": \"JSON Schema for hapi server configuration options passed to Hapi.server().\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"host\": {\n      \"type\": \"string\",\n      \"default\": \"localhost\",\n      \"description\": \"Public hostname or IP address.\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"default\": 3000,\n      \"description\": \"TCP port to listen on.\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname or IP address to bind to (defaults to host).\"\n    },\n    \"autoListen\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Whether to automatically start listening.\"\n    },\n    \"tls\": {\n      \"oneOf\": [\n        { \"type\"\
  : \"boolean\" },\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"key\": { \"type\": \"string\" },\n            \"cert\": { \"type\": \"string\" },\n            \"ca\": {\n              \"type\": \"array\",\n              \"items\": { \"type\": \"string\" }\n            }\n          }\n        }\n      ],\n      \"description\": \"TLS configuration.\"\n    },\n    \"routes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"cors\": {\n          \"oneOf\": [\n            { \"type\": \"boolean\" },\n            {\n              \"type\": \"object\",\n              \"properties\": {\n                \"origin\": {\n                  \"type\": \"array\",\n                  \"items\": { \"type\": \"string\" },\n                  \"default\": [\"*\"]\n                },\n                \"maxAge\": {\n                  \"type\": \"integer\",\n                  \"default\": 86400\n                },\n                \"headers\": {\n    \
  \              \"type\": \"array\",\n                  \"items\": { \"type\": \"string\" }\n                },\n                \"additionalHeaders\": {\n                  \"type\": \"array\",\n                  \"items\": { \"type\": \"string\" }\n                },\n                \"credentials\": {\n                  \"type\": \"boolean\",\n                  \"default\": false\n                }\n              }\n            }\n          ],\n          \"description\": \"CORS configuration.\"\n        },\n        \"files\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"relativeTo\": {\n              \"type\": \"string\",\n              \"description\": \"Base path for relative file paths.\"\n            }\n          }\n        },\n        \"validate\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"failAction\": {\n              \"type\": \"string\",\n              \"enum\": [\"error\", \"log\", \"ignore\"],\n        \
  \      \"default\": \"error\"\n            }\n          }\n        },\n        \"security\": {\n          \"oneOf\": [\n            { \"type\": \"boolean\" },\n            {\n              \"type\": \"object\",\n              \"properties\": {\n                \"hsts\": {\n                  \"oneOf\": [\n                    { \"type\": \"boolean\" },\n                    {\n                      \"type\": \"object\",\n                      \"properties\": {\n                        \"maxAge\": { \"type\": \"integer\" },\n                        \"includeSubDomains\": { \"type\": \"boolean\" },\n                        \"preload\": { \"type\": \"boolean\" }\n                      }\n                    }\n                  ]\n                },\n                \"xframe\": {\n                  \"oneOf\": [\n                    { \"type\": \"boolean\" },\n                    { \"type\": \"string\", \"enum\": [\"deny\", \"sameorigin\"] }\n                  ]\n                },\n        \
  \        \"xss\": { \"type\": \"boolean\" },\n                \"noOpen\": { \"type\": \"boolean\" },\n                \"noSniff\": { \"type\": \"boolean\" },\n                \"referrer\": { \"type\": \"boolean\" }\n              }\n            }\n          ],\n          \"description\": \"Security header configuration.\"\n        }\n      },\n      \"description\": \"Default route configuration.\"\n    },\n    \"cache\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": { \"type\": \"string\" },\n            \"provider\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"constructor\": { \"type\": \"string\" },\n                \"options\": { \"type\": \"object\" }\n              }\n            }\n          }\n        },\n        {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"object\" }\n        }\n      ],\n      \"description\"\
  : \"Server-side cache provider configuration.\"\n    },\n    \"compression\": {\n      \"oneOf\": [\n        { \"type\": \"boolean\" },\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"minBytes\": {\n              \"type\": \"integer\",\n              \"default\": 1024,\n              \"description\": \"Minimum response size in bytes to compress.\"\n            }\n          }\n        }\n      ],\n      \"description\": \"Compression settings.\"\n    },\n    \"debug\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"request\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"Request event tags to log.\"\n        },\n        \"log\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"Server log event tags to log.\"\n        }\n      },\n      \"description\": \"Debug logging configuration.\"\n    },\n    \"\
  load\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"sampleInterval\": {\n          \"type\": \"integer\",\n          \"default\": 0,\n          \"description\": \"Sampling interval for load monitoring in milliseconds.\"\n        },\n        \"maxHeapUsedBytes\": {\n          \"type\": \"integer\",\n          \"default\": 0,\n          \"description\": \"Maximum V8 heap used in bytes (0 = no limit).\"\n        },\n        \"maxRssBytes\": {\n          \"type\": \"integer\",\n          \"default\": 0,\n          \"description\": \"Maximum process RSS in bytes (0 = no limit).\"\n        },\n        \"maxEventLoopDelay\": {\n          \"type\": \"integer\",\n          \"default\": 0,\n          \"description\": \"Maximum event loop delay in milliseconds (0 = no limit).\"\n        }\n      },\n      \"description\": \"Server load monitoring configuration.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hapi/refs/heads/main/json-schema/hapi-server-configuration.json
tags:
- Authentication
- Frameworks
- JavaScript
- Node.js
- Validation
- Web Framework
title: hapi Server Configuration
---
