---
description: JSON Schema for Gin web framework router engine configuration and common middleware settings.
layout: schema
name: Gin Router and Middleware Configuration
properties_list:
- description: Gin mode (set via GIN_MODE env var or gin.SetMode()).
  name: mode
  type: string
- description: Redirect /foo/ to /foo or vice versa.
  name: redirectTrailingSlash
  type: boolean
- description: Try to fix and redirect the request path.
  name: redirectFixedPath
  type: boolean
- description: Return 405 instead of 404 for mismatched methods.
  name: handleMethodNotAllowed
  type: boolean
- description: Parse client IP from X-Forwarded-For / X-Real-IP.
  name: forwardedByClientIP
  type: boolean
- description: Use url.RawPath for route matching.
  name: useRawPath
  type: boolean
- description: Unescape path values for matching.
  name: unescapePathValues
  type: boolean
- description: Remove extra slashes from URL path.
  name: removeExtraSlash
  type: boolean
- description: Maximum memory for multipart forms in bytes (default 32MB).
  name: maxMultipartMemory
  type: integer
- description: Trusted platform header (e.g., X-Forwarded-For).
  name: trustedPlatform
  type: string
- description: List of trusted proxy CIDR ranges.
  name: trustedProxies
  type: array
- description: Common middleware configuration.
  name: middleware
  type: object
provider_name: Gin
provider_slug: gin
schema_file: json-schema/gin-configuration.json
slug: gin-configuration
source_filename: gin-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/gin/json-schema/gin-configuration.json\",\n  \"title\": \"Gin Router and Middleware Configuration\",\n  \"description\": \"JSON Schema for Gin web framework router engine configuration and common middleware settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mode\": {\n      \"type\": \"string\",\n      \"enum\": [\"debug\", \"release\", \"test\"],\n      \"default\": \"debug\",\n      \"description\": \"Gin mode (set via GIN_MODE env var or gin.SetMode()).\"\n    },\n    \"redirectTrailingSlash\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Redirect /foo/ to /foo or vice versa.\"\n    },\n    \"redirectFixedPath\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Try to fix and redirect the request path.\"\n    },\n    \"handleMethodNotAllowed\": {\n      \"type\": \"boolean\"\
  ,\n      \"default\": false,\n      \"description\": \"Return 405 instead of 404 for mismatched methods.\"\n    },\n    \"forwardedByClientIP\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Parse client IP from X-Forwarded-For / X-Real-IP.\"\n    },\n    \"useRawPath\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Use url.RawPath for route matching.\"\n    },\n    \"unescapePathValues\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Unescape path values for matching.\"\n    },\n    \"removeExtraSlash\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Remove extra slashes from URL path.\"\n    },\n    \"maxMultipartMemory\": {\n      \"type\": \"integer\",\n      \"default\": 33554432,\n      \"description\": \"Maximum memory for multipart forms in bytes (default 32MB).\"\n    },\n    \"trustedPlatform\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Trusted platform header (e.g., X-Forwarded-For).\"\n    },\n    \"trustedProxies\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"List of trusted proxy CIDR ranges.\"\n    },\n    \"middleware\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"logger\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"enabled\": {\n              \"type\": \"boolean\",\n              \"default\": true,\n              \"description\": \"Enable request logging middleware.\"\n            },\n            \"formatter\": {\n              \"type\": \"string\",\n              \"description\": \"Custom log format string.\"\n            },\n            \"output\": {\n              \"type\": \"string\",\n              \"description\": \"Log output destination.\"\n            },\n            \"skipPaths\": {\n              \"type\": \"array\",\n              \"items\": { \"type\": \"string\"\
  \ },\n              \"description\": \"Paths to skip logging.\"\n            }\n          }\n        },\n        \"recovery\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"enabled\": {\n              \"type\": \"boolean\",\n              \"default\": true,\n              \"description\": \"Enable panic recovery middleware.\"\n            }\n          }\n        },\n        \"cors\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"allowOrigins\": {\n              \"type\": \"array\",\n              \"items\": { \"type\": \"string\" },\n              \"default\": [\"*\"],\n              \"description\": \"Allowed origins.\"\n            },\n            \"allowMethods\": {\n              \"type\": \"array\",\n              \"items\": { \"type\": \"string\" },\n              \"description\": \"Allowed HTTP methods.\"\n            },\n            \"allowHeaders\": {\n              \"type\": \"array\",\n              \"items\"\
  : { \"type\": \"string\" },\n              \"description\": \"Allowed request headers.\"\n            },\n            \"exposeHeaders\": {\n              \"type\": \"array\",\n              \"items\": { \"type\": \"string\" },\n              \"description\": \"Headers exposed to the client.\"\n            },\n            \"allowCredentials\": {\n              \"type\": \"boolean\",\n              \"default\": false,\n              \"description\": \"Allow credentials.\"\n            },\n            \"maxAge\": {\n              \"type\": \"integer\",\n              \"description\": \"Preflight cache duration in seconds.\"\n            }\n          }\n        },\n        \"rateLimiter\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"enabled\": {\n              \"type\": \"boolean\",\n              \"default\": false,\n              \"description\": \"Enable rate limiting middleware.\"\n            },\n            \"limit\": {\n              \"type\": \"integer\"\
  ,\n              \"description\": \"Maximum requests per period.\"\n            },\n            \"period\": {\n              \"type\": \"string\",\n              \"description\": \"Rate limit period duration.\"\n            }\n          }\n        }\n      },\n      \"description\": \"Common middleware configuration.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gin/refs/heads/main/json-schema/gin-configuration.json
tags:
- Microservices
title: Gin Router and Middleware Configuration
---
