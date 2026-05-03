---
description: JSON Schema for Resilience4j TimeLimiter configuration properties used in application.yml or application.properties.
layout: schema
name: Resilience4j Time Limiter Configuration
properties_list:
- description: ''
  name: resilience4j
  type: object
provider_name: Resilience4j
provider_slug: resilience4j
schema_file: json-schema/time-limiter-configuration.json
slug: time-limiter-configuration
source_filename: time-limiter-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/resilience4j/json-schema/time-limiter-configuration.json\",\n  \"title\": \"Resilience4j Time Limiter Configuration\",\n  \"description\": \"JSON Schema for Resilience4j TimeLimiter configuration properties used in application.yml or application.properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resilience4j\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"timelimiter\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"configs\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"$ref\": \"#/$defs/TimeLimiterConfig\"\n              }\n            },\n            \"instances\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"$ref\": \"#/$defs/TimeLimiterInstance\"\n              }\n          \
  \  }\n          }\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"TimeLimiterConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"timeoutDuration\": {\n          \"type\": \"string\",\n          \"default\": \"1s\",\n          \"description\": \"Configurable timeout duration. Defaults to 1 second.\"\n        },\n        \"cancelRunningFuture\": {\n          \"type\": \"boolean\",\n          \"default\": true,\n          \"description\": \"Whether to cancel the running Future after a timeout. Defaults to true.\"\n        }\n      }\n    },\n    \"TimeLimiterInstance\": {\n      \"allOf\": [\n        { \"$ref\": \"#/$defs/TimeLimiterConfig\" },\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"baseConfig\": {\n              \"type\": \"string\",\n              \"description\": \"Name of a shared configuration to inherit from.\"\n            }\n          }\n        }\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/resilience4j/refs/heads/main/json-schema/time-limiter-configuration.json
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
title: Resilience4j Time Limiter Configuration
---
