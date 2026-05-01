---
description: JSON Schema for Fastify server instance options and plugin configuration patterns.
layout: schema
name: Fastify Plugin and Server Configuration
properties_list:
- description: Logger configuration (Pino).
  name: logger
  type: object
- description: Ajv (JSON Schema validator) configuration.
  name: ajv
  type: object
- description: Enable HTTP/2 support.
  name: http2
  type: boolean
- description: HTTPS/TLS configuration.
  name: https
  type: object
- description: Connection timeout in milliseconds.
  name: connectionTimeout
  type: integer
- description: Keep-alive timeout in milliseconds.
  name: keepAliveTimeout
  type: integer
- description: Maximum parameter length for URL params.
  name: maxParamLength
  type: integer
- description: Default maximum body size in bytes.
  name: bodyLimit
  type: integer
- description: Case-sensitive routing.
  name: caseSensitive
  type: boolean
- description: Ignore trailing slashes in routes.
  name: ignoreTrailingSlash
  type: boolean
- description: Ignore duplicate slashes in routes.
  name: ignoreDuplicateSlashes
  type: boolean
- description: Disable automatic request logging.
  name: disableRequestLogging
  type: boolean
- description: Header name to use for request ID.
  name: requestIdHeader
  type: string
- description: Label for request ID in logs.
  name: requestIdLogLabel
  type: string
- description: Plugin load timeout in milliseconds.
  name: pluginTimeout
  type: integer
- description: Force close connections on server close.
  name: forceCloseConnections
  type: object
- description: Trust proxy configuration.
  name: trustProxy
  type: object
- description: Return 503 when server is closing.
  name: return503OnClosing
  type: boolean
provider_name: Fastify
provider_slug: fastify
schema_file: json-schema/fastify-plugin-config.json
slug: fastify-plugin-config
source_filename: fastify-plugin-config.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/fastify/json-schema/fastify-plugin-config.json\",\n  \"title\": \"Fastify Plugin and Server Configuration\",\n  \"description\": \"JSON Schema for Fastify server instance options and plugin configuration patterns.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"logger\": {\n      \"description\": \"Logger configuration (Pino).\",\n      \"oneOf\": [\n        { \"type\": \"boolean\" },\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"level\": {\n              \"type\": \"string\",\n              \"enum\": [\"trace\", \"debug\", \"info\", \"warn\", \"error\", \"fatal\", \"silent\"],\n              \"default\": \"info\"\n            },\n            \"prettyPrint\": {\n              \"type\": \"boolean\",\n              \"description\": \"Enable pretty printing (dev only).\",\n              \"default\": false\n      \
  \      },\n            \"serializers\": {\n              \"type\": \"object\",\n              \"description\": \"Custom serializers for log fields.\",\n              \"additionalProperties\": true\n            },\n            \"redact\": {\n              \"type\": \"array\",\n              \"description\": \"Paths to redact from logs.\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"file\": {\n              \"type\": \"string\",\n              \"description\": \"Log output file path.\"\n            },\n            \"transport\": {\n              \"type\": \"object\",\n              \"description\": \"Pino transport configuration.\",\n              \"properties\": {\n                \"target\": {\n                  \"type\": \"string\"\n                },\n                \"options\": {\n                  \"type\": \"object\",\n                  \"additionalProperties\": true\n                }\n              },\n     \
  \         \"additionalProperties\": true\n            }\n          },\n          \"additionalProperties\": true\n        }\n      ]\n    },\n    \"ajv\": {\n      \"type\": \"object\",\n      \"description\": \"Ajv (JSON Schema validator) configuration.\",\n      \"properties\": {\n        \"customOptions\": {\n          \"type\": \"object\",\n          \"description\": \"Custom Ajv options.\",\n          \"properties\": {\n            \"removeAdditional\": {\n              \"type\": \"boolean\",\n              \"default\": false\n            },\n            \"useDefaults\": {\n              \"type\": \"boolean\",\n              \"default\": true\n            },\n            \"coerceTypes\": {\n              \"type\": \"boolean\",\n              \"default\": true\n            },\n            \"allErrors\": {\n              \"type\": \"boolean\",\n              \"default\": false\n            }\n          },\n          \"additionalProperties\": true\n        },\n        \"plugins\": {\n\
  \          \"type\": \"array\",\n          \"description\": \"Ajv plugins to load.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"http2\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable HTTP/2 support.\",\n      \"default\": false\n    },\n    \"https\": {\n      \"type\": \"object\",\n      \"description\": \"HTTPS/TLS configuration.\",\n      \"properties\": {\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"Path to TLS private key or key contents.\"\n        },\n        \"cert\": {\n          \"type\": \"string\",\n          \"description\": \"Path to TLS certificate or certificate contents.\"\n        },\n        \"allowHTTP1\": {\n          \"type\": \"boolean\",\n          \"description\": \"Allow HTTP/1.1 fallback with HTTP/2.\",\n          \"default\": true\n        }\n      },\n      \"additionalProperties\": true\n    },\n  \
  \  \"connectionTimeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Connection timeout in milliseconds.\",\n      \"default\": 0\n    },\n    \"keepAliveTimeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Keep-alive timeout in milliseconds.\",\n      \"default\": 72000\n    },\n    \"maxParamLength\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum parameter length for URL params.\",\n      \"default\": 100\n    },\n    \"bodyLimit\": {\n      \"type\": \"integer\",\n      \"description\": \"Default maximum body size in bytes.\",\n      \"default\": 1048576\n    },\n    \"caseSensitive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Case-sensitive routing.\",\n      \"default\": true\n    },\n    \"ignoreTrailingSlash\": {\n      \"type\": \"boolean\",\n      \"description\": \"Ignore trailing slashes in routes.\",\n      \"default\": false\n    },\n    \"ignoreDuplicateSlashes\": {\n      \"type\": \"boolean\",\n      \"\
  description\": \"Ignore duplicate slashes in routes.\",\n      \"default\": false\n    },\n    \"disableRequestLogging\": {\n      \"type\": \"boolean\",\n      \"description\": \"Disable automatic request logging.\",\n      \"default\": false\n    },\n    \"requestIdHeader\": {\n      \"type\": \"string\",\n      \"description\": \"Header name to use for request ID.\",\n      \"default\": \"request-id\"\n    },\n    \"requestIdLogLabel\": {\n      \"type\": \"string\",\n      \"description\": \"Label for request ID in logs.\",\n      \"default\": \"reqId\"\n    },\n    \"pluginTimeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Plugin load timeout in milliseconds.\",\n      \"default\": 10000\n    },\n    \"forceCloseConnections\": {\n      \"description\": \"Force close connections on server close.\",\n      \"oneOf\": [\n        { \"type\": \"boolean\" },\n        { \"type\": \"string\", \"const\": \"idle\" }\n      ],\n      \"default\": \"idle\"\n    },\n    \"trustProxy\"\
  : {\n      \"description\": \"Trust proxy configuration.\",\n      \"oneOf\": [\n        { \"type\": \"boolean\" },\n        { \"type\": \"string\" },\n        { \"type\": \"integer\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"default\": false\n    },\n    \"return503OnClosing\": {\n      \"type\": \"boolean\",\n      \"description\": \"Return 503 when server is closing.\",\n      \"default\": true\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fastify/refs/heads/main/json-schema/fastify-plugin-config.json
tags:
- Frameworks
- High Performance
- JavaScript
- JSON Schema
- Node.js
- TypeScript
title: Fastify Plugin and Server Configuration
---
