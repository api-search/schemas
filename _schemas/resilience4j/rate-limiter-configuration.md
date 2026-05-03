---
description: JSON Schema for Resilience4j rate limiter configuration properties.
layout: schema
name: Resilience4j Rate Limiter Configuration
properties_list:
- description: ''
  name: resilience4j
  type: object
provider_name: Resilience4j
provider_slug: resilience4j
schema_file: json-schema/rate-limiter-configuration.json
slug: rate-limiter-configuration
source_filename: rate-limiter-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/resilience4j/json-schema/rate-limiter-configuration.json\",\n  \"title\": \"Resilience4j Rate Limiter Configuration\",\n  \"description\": \"JSON Schema for Resilience4j rate limiter configuration properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resilience4j\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ratelimiter\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"configs\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"$ref\": \"#/$defs/RateLimiterConfig\"\n              }\n            },\n            \"instances\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"$ref\": \"#/$defs/RateLimiterInstance\"\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n\
  \  \"$defs\": {\n    \"RateLimiterConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"limitForPeriod\": {\n          \"type\": \"integer\",\n          \"default\": 50,\n          \"description\": \"Number of permissions available during one limit refresh period.\"\n        },\n        \"limitRefreshPeriod\": {\n          \"type\": \"string\",\n          \"default\": \"500ns\",\n          \"description\": \"Duration of a limit refresh period.\"\n        },\n        \"timeoutDuration\": {\n          \"type\": \"string\",\n          \"default\": \"5s\",\n          \"description\": \"Default wait time for permission.\"\n        },\n        \"registerHealthIndicator\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Whether to register a health indicator.\"\n        },\n        \"eventConsumerBufferSize\": {\n          \"type\": \"integer\",\n          \"default\": 100,\n          \"description\": \"Size of the event\
  \ consumer buffer.\"\n        },\n        \"writableStackTraceEnabled\": {\n          \"type\": \"boolean\",\n          \"default\": true,\n          \"description\": \"Whether RequestNotPermitted has a writable stack trace.\"\n        }\n      }\n    },\n    \"RateLimiterInstance\": {\n      \"allOf\": [\n        { \"$ref\": \"#/$defs/RateLimiterConfig\" },\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"baseConfig\": {\n              \"type\": \"string\",\n              \"description\": \"Name of a shared configuration to inherit from.\"\n            }\n          }\n        }\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/resilience4j/refs/heads/main/json-schema/rate-limiter-configuration.json
tags:
- Bulkhead
- Circuit Breaker
- Fault Tolerance
- Java
- Microservices
- Rate Limiter
- Resilience
- Retry
- Spring Boot
- Functional Programming
title: Resilience4j Rate Limiter Configuration
---
